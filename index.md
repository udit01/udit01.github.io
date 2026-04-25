---
layout: home
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_home

# image for page specific usage
img: ":home-heading.jpg"
# publish date (used for seo)
# if not specified, site.time will be used.
#date: 2022-03-03 12:32:00 +0000

# for override items in _data/lang/[language].yml
#title: My title
#button_name: "My button"
# for override side_and_top_nav_buttons in _data/conf/main.yml
#icon: "fa fa-bath"

# seo
# if not specified, date will be used.
#meta_modify_date: 2022-03-03 12:32:00 +0000
# check the meta_common_description in _data/owner/[language].yml
#meta_description: ""

# optional
# please use the "image_viewer_on" below to enable image viewer for individual pages or posts (_posts/ or [language]/_posts folders).
# image viewer can be enabled or disabled for all posts using the "image_viewer_posts: true" setting in _data/conf/main.yml.
#image_viewer_on: true
# please use the "image_lazy_loader_on" below to enable image lazy loader for individual pages or posts (_posts/ or [language]/_posts folders).
# image lazy loader can be enabled or disabled for all posts using the "image_lazy_loader_posts: true" setting in _data/conf/main.yml.
#image_lazy_loader_on: true
# exclude from on site search
#on_site_search_exclude: true
# exclude from search engines
#search_engine_exclude: true
# to disable this page, simply set published: false or delete this file
# don't forget that this is root index.html. If you disable this, there will be no index.html page to open
#published: false
---

{%- comment -%} Please delete below and place your page content here {%- endcomment -%}

{%- include util/auto-content-generator.liquid -%}

# Building the Next Generation of Agentic AI

Welcome! I am **Udit Jain**, an Agentic AI Engineer at the **AI Core Team, Samsung Research**, focused on the frontier of large language model post-training and autonomous agent systems.

## What I Work On

My current work lives at the intersection of post-training research and production-scale AI:
- **LLM Post-Training**: RLHF, DPO, SFT pipelines for instruction-following and alignment
- **Reinforcement Learning for LLMs**: Reward modeling, policy optimization, and RL-based fine-tuning
- **Knowledge Distillation**: Transferring capabilities from frontier models to efficient, deployable targets
- **Agentic Evaluation**: Building multi-turn agent benchmarks and evaluation pipelines for complex reasoning tasks
- **Training Infrastructure**: Distributed training with NeMo, large-scale inference with vLLM

Previously, I led computer vision R&D for Samsung's next-generation smart appliances, shipped on-device AI models to millions of users, and built health data pipelines over Samsung Health's 200M+ user dataset.

Please explore my [Projects](/tabs/projects), read about my [Professional Journey](/tabs/about), or view my [Resume & Skills](/tabs/links).
