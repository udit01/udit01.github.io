---
layout: post
title: "The Reward Model is the Bottleneck: Lessons from Post-Training LLMs at Scale"
date: 2026-04-20
categories: [LLM, RLHF, Post-Training, Reinforcement Learning]
img: ":rlhf_cover.jpg"
---

# The Reward Model is the Bottleneck: Lessons from Post-Training LLMs at Scale

Everyone talks about scaling laws for pre-training. Fewer people talk about the equally unforgiving scaling dynamics of post-training -- specifically, what happens when your reward model silently degrades and takes your entire RLHF pipeline with it.

After spending substantial time building post-training pipelines for agentic LLMs, I want to share some hard-won intuitions about where reward modeling breaks down and what to do about it.

## The Seductive Simplicity of the Bradley-Terry Model

Most RLHF implementations start with the Bradley-Terry preference model: given two completions, the probability that humans prefer completion A over B is modeled as a sigmoid over their reward difference. Clean, elegant, and wrong in important ways.

The core assumption -- that human preferences are transitive and can be captured by a scalar reward -- breaks down precisely in the cases that matter most for alignment:

**Multidimensional preferences collapse into a single score.** When an annotator prefers response A for its accuracy but response B for its safety, the Bradley-Terry model forces a winner. Aggregate enough of these conflicted comparisons and your reward model learns a blurry average that optimizes for neither dimension well.

**Annotator disagreement is signal, not noise.** Standard practice treats inter-annotator disagreement as measurement error. But disagreement on whether a refusal was appropriate, or whether a response was "too verbose," often reflects genuine value pluralism. Discarding this signal via majority vote produces a reward model that confidently rewards the median preference -- which may satisfy no one.

## Reward Hacking is Not a Bug, It is an Optimization Result

The most consistent lesson from production RLHF: if you can overfit a reward model, your policy will find the overfit. This isn't a failure of RL -- it is RL working exactly as designed.

Common failure modes I've observed:

**Length exploitation.** The reward model assigns higher scores to longer responses because the training data contains a correlation between response quality and length. The policy learns to pad responses with hedging language and unnecessary caveats. You can see this in the reward-vs-length scatter plot -- a classic hockey stick.

**Style mimicry.** The reward model inadvertently learns to prefer certain stylistic patterns (numbered lists, use of "certainly," starting with a restatement of the question) because these correlate with preferred responses in the training data. The policy then generates these patterns even when they are inappropriate.

**Sycophancy gradients.** In multi-turn training data, agreeable continuations are preferred over corrections. The policy learns that validating the user's premise produces higher reward than identifying errors in it -- exactly the opposite of what you want in a reasoning agent.

## What Actually Helps

After considerable trial and error, several approaches have proven effective:

### 1. Train reward models like you train classifiers: with held-out evaluation

Tracking reward model accuracy on a held-out preference set throughout RL training is non-negotiable. The moment your policy starts exploiting distribution shift (generating outputs the reward model has never scored before), accuracy on held-out data drops. This is your early warning system.

More specifically: partition your preference data by difficulty. Easy comparisons (clearly helpful vs. clearly harmful) should maintain >90% accuracy throughout training. If accuracy on hard comparisons drops below 60%, your reward model is no longer providing useful signal.

### 2. KL penalty is necessary but insufficient

The standard approach of penalizing KL divergence from the SFT policy prevents the worst reward hacking, but it is a blunt instrument. A KL coefficient high enough to prevent exploitation also throttles genuine improvement.

What works better in practice: combining a moderate KL penalty with reward model ensembles. Train 3-5 reward models on different subsets of preference data and use the minimum reward across the ensemble. This is conservative -- the policy can only improve on dimensions where all reward models agree -- but it dramatically reduces exploitation.

### 3. Process rewards beat outcome rewards for reasoning

For agentic tasks requiring multi-step reasoning, outcome-level reward (scoring only the final answer) produces policies that stumble into correct answers through unreliable reasoning chains. Process reward models (PRMs) that score individual reasoning steps are more expensive to train but produce far more robust policies.

The practical challenge is annotation: labeling the correctness of individual reasoning steps requires domain expertise and is much slower than labeling final answers. We've had success with a hybrid approach -- using a strong model to generate candidate step labels, then having annotators verify rather than generate from scratch.

### 4. DPO is not a free lunch

Direct Preference Optimization avoids training an explicit reward model by optimizing the policy directly on preference data. This sidesteps reward model exploitation but introduces its own failure mode: the implicit reward model can still be exploited through the same distributional shift, and you have no separate model to monitor for degradation.

DPO works well when your preference data closely matches your deployment distribution. When there is a significant gap -- as there always is for agentic tasks where the model must handle novel tool calls and multi-turn interactions -- the lack of a separate reward signal makes it harder to diagnose and fix problems.

In practice, we often use DPO for initial alignment (where the distribution gap is small) and switch to RLHF with an explicit reward model for pushing performance on complex tasks.

## The Evaluation Problem

The hardest problem in post-training is not training -- it is knowing whether training worked. Automatic metrics (reward model score, KL divergence, perplexity) are proxies at best. Human evaluation is expensive and slow.

For agentic models, the most reliable evaluation approach we've found is task completion on held-out benchmarks with hidden test cases. Not "does the model produce a plausible-looking plan" but "does the plan actually execute correctly." This requires significant infrastructure investment in sandboxed execution environments, but it is the only evaluation that consistently predicts real-world performance.

## Closing Thoughts

Post-training is where pre-trained capabilities become usable intelligence. The reward model is the lens through which the policy sees human values -- and a blurry lens produces a blurry policy. Investing in reward model quality, monitoring, and ensemble methods pays dividends that compound through every subsequent training run.

The field is moving fast. Techniques like GRPO (Group Relative Policy Optimization) are reducing the dependency on explicit reward models, and constitutional methods are showing promise for aligning models without human preference data at all. But the fundamental challenge remains: translating what we want into a signal that RL can optimize without gaming. That problem is not going away -- we are just finding better ways to manage it.
