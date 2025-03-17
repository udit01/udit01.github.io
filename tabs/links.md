---
layout: links
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_links

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
#published: false


# you can always move this content to _data/content/ folder
# just create new file at _data/content/links/[language].yml and move content below.
###########################################################
#                Links Page Data
###########################################################
page_data:
  main:
    header: "Professional Resources"
    info: "Publications, Education, Skills, Media Coverage & More"

  # To change order of the Categories, simply change order. (you don't need to change list order.)
  category:
    - title: "Resume & Education"
      type: id_resume
      color: "green"
    - title: "Publications & Research"
      type: id_pub
      color: "#F4A273"
    - title: "Media Coverage"
      type: id_media
      color: "#14A273"
    - title: "Technical Skills"
      type: id_skills
      color: "yellow"
    - title: "Certifications"
      type: id_cert
      color: "orange"
    - title: "Recommended Resources"
      type: id_rr
      color: "gray"

  list:
    - type: id_resume
      title: "Udit Jain - Comprehensive Resume"
      url: "https://drive.google.com/file/d/1hp81IaoKNDYjjmG2tCerTp56EoJQgVad/view?usp=sharing"
      info: "My detailed professional resume highlighting experience at Samsung Research, academic achievements, and technical expertise in AI, computer vision, and software development."
    
    - type: id_resume
      title: "Education: Indian Institute of Technology, Delhi"
      url: "https://www.iitd.ac.in/"
      info: "B.Tech in Computer Science and Engineering (2016-2020) with a CGPA of 9.10/10.0. Specialized in artificial intelligence, computer vision, and systems programming."
    
    - type: id_resume
      title: "International Experience"
      url: ""
      info: "Research internships at Harvard University (USA), Samsung Research (South Korea), and Kyutech Institute of Technology (Japan), providing a global perspective on technology development and cross-cultural collaboration."
    
    - type: id_pub
      title: "APEX: Adaptive Ext4 File System for Enhanced Data Recoverability in Edge Devices"
      url: "https://arxiv.org/abs/1910.01642"
      info: "Co-authored research paper published in the Proceedings of the 11th IEEE International Conference on Cloud Computing, Sydney, Australia, 2019. This work presents a novel file system design that significantly improves data recovery capabilities for edge computing devices through reinforcement learning techniques."
    
    - type: id_pub
      title: "Transformative Effects of IoT, Blockchain and Artificial Intelligence on Cloud Computing"
      url: "https://arxiv.org/abs/1911.01941"
      info: "Co-authored research paper published in Distributed, Parallel, and Cluster Computing (cs.DC) 2019. This comprehensive analysis explores how emerging technologies are reshaping cloud computing architectures, with particular focus on integration challenges and future directions."
    
    - type: id_pub
      title: "Two-Color Disjunctive Rado Number for Systems of Linear Equations"
      url: ""
      info: "(Under Review) Advanced mathematical research exploring combinatorial number theory. Developed novel algorithms for solving complex coloring problems in systems of linear equations, contributing to the theoretical understanding of Ramsey theory and its applications."
    
    - type: id_pub
      title: "Elderly Clothing Assistance Robotics Research"
      url: "https://tom-shibata.hatenablog.com/entry/2018/06/16/073923"
      info: "Research featured on Professor Shibata's blog detailing our innovative robotic system for elderly care. The BAXTER robot implementation was showcased at RoboMech 2018/2019 and iREX 2019 exhibitions, receiving coverage on Japanese National Television for its societal impact."

    - type: id_media
      title: "Samsung AI Inside Refrigerator - Developer Story"
      url: "https://www.youtube.com/watch?v=239uUZCIuqU"
      info: "Official Samsung video featuring the AI-powered smart refrigerator technology I helped develop. The video demonstrates how computer vision and on-device AI enable food recognition, inventory management, and personalized recommendations to transform the kitchen experience."

    - type: id_media
      title: "Samsung Bespoke 4-Door Refrigerator with AI Features"
      url: "https://www.youtube.com/watch?v=Pm4CTT0rhvA"
      info: "Product showcase of Samsung's Bespoke refrigerator featuring the AI vision system I helped develop. The video highlights how the integrated camera and recognition technology enhance user convenience through automated food detection."

    - type: id_media
      title: "CES 2024: Samsung Showcases AI-Based Home Appliances"
      url: "https://news.samsung.com/global/ces-2024-elevating-lifestyles-samsung-showcases-ai-based-home-appliances-at-the-home-experience-zone"
      info: "Samsung Newsroom coverage of the CES 2024 exhibition featuring the AI-powered appliances I contributed to. The article details how these smart devices are transforming home environments through intelligent automation and personalization."

    - type: id_media
      title: "Understanding Sleep: How Our Sleeping Habits Changed Over the Pandemic"
      url: "https://news.samsung.com/global/understanding-sleep-how-our-sleeping-habits-changed-over-the-pandemic"
      info: "Samsung Newsroom feature based on my data analysis work with the Samsung Health team. This article presents key findings from our comprehensive study of sleep patterns before, during, and after the COVID-19 pandemic, revealing significant global behavioral shifts."

    - type: id_media
      title: "Global Sleep Health Study - MBC News Coverage"
      url: "https://www.youtube.com/watch?v=6yaVXXMIb6o"
      info: "Korean national television (MBC) news segment covering our Samsung Health sleep research. The report highlights how our analysis of anonymized data from millions of users provided unprecedented insights into global sleep health trends during the pandemic."

    - type: id_media
      title: "Interview: Sleep Scientist Dr. Vanessa Hill on Technology and Sleep Optimization"
      url: "https://news.samsung.com/global/interview-sleep-scientist-dr-vanessa-hill-explains-how-technology-can-help-users-optimize-their-sleep"
      info: "Expert interview complementing our Samsung Health sleep research. Dr. Hill discusses how the data analysis I contributed to is helping advance understanding of sleep patterns and how technology can be leveraged to improve sleep quality."

    - type: id_media
      title: "Samsung Health Research Stack Wins UX Design Award 2023"
      url: "https://research.samsung.com/news/Samsung-Health-Stack-Wins-UX-Design-Award-2023-for-Design-Excellence"
      info: "Recognition for the Samsung Health Research platform I helped develop. The award highlights the innovative user experience design that makes complex health data collection and visualization accessible to medical researchers."

    - type: id_skills
      title: "Artificial Intelligence & Computer Vision"
      url: ""
      info: "• Deep Learning frameworks: TensorFlow, PyTorch, Keras\n• Computer Vision: OpenCV, object detection, segmentation, feature matching\n• Model Optimization: TensorFlow Lite, quantization, knowledge distillation\n• NPU Development: vsi-acuity toolkit, on-device AI optimization\n• Natural Language Processing: SpaCy, NLTK, KlonPY, OpenIE, StanfordIE\n• Specialized Techniques: Monte Carlo simulation, inverse rendering, GPU acceleration"
    
    - type: id_skills
      title: "Cloud & Data Engineering"
      url: ""
      info: "• AWS Ecosystem: S3, EMR, Glue, Athena, IAM, CLI\n• Big Data Processing: Spark, Hadoop, PySpark\n• Data Formats: Avro, Parquet, JSON\n• Database Systems: SQL, NoSQL, RoomDB\n• Data Visualization: Apache Superset, Matplotlib, Seaborn\n• Statistical Analysis: Time series forecasting, A/B testing, significance testing\n• Google Cloud: BigQuery, Cloud Storage"
    
    - type: id_skills
      title: "Software Development"
      url: ""
      info: "• Programming Languages: Python, Java, Kotlin, C/C++, Assembly\n• Mobile Development: Android SDK, Jetpack Compose, Firebase\n• Architecture: Clean Architecture, MVVM, microservices\n• Web Technologies: Node.js, Django, RESTful APIs\n• Version Control: Git, GitHub\n• DevOps: Docker, CI/CD pipelines\n• Testing: Unit testing, integration testing, TDD"
    
    - type: id_skills
      title: "Robotics & Specialized Systems"
      url: ""
      info: "• Robotics: ROS (Robot Operating System), Baxter robot programming\n• 3D Sensing: Kinect, point cloud processing, depth cameras\n• Embedded Systems: Edge computing, microcontroller programming\n• Operating Systems: Linux kernel development, FreeBSD optimization\n• FPGA Programming: Vivado Design Suite, Xilinx ISE\n• IoT Development: Sensor integration, data collection pipelines"
    
    - type: id_cert
      title: "Data Science Level 2 Certification"
      url: ""
      info: "Samsung Electronics, 2023. Advanced certification in data science methodologies, statistical analysis, and machine learning applications for large-scale data processing and insights generation."
    
    - type: id_cert
      title: "Professional Certification in AI Development"
      url: ""
      info: "Samsung Electronics, 2021. Comprehensive certification covering deep learning architectures, computer vision algorithms, model optimization, and deployment strategies for production AI systems."
    
    - type: id_cert
      title: "Professional Certification in Cloud Architecture"
      url: ""
      info: "Samsung Electronics, 2021. Specialized certification in designing and implementing cloud-based systems, with focus on scalability, security, and integration with AI/ML workflows."
    
    - type: id_cert
      title: "Korean Language Proficiency"
      url: ""
      info: "Certificate of Excellence, Seoul National University Level 3-4 Korean Language Program, 2023-2024. Demonstrates intermediate proficiency in both written and spoken Korean, facilitating effective communication in professional settings."

    - type: id_rr
      title: "Brandon Rohrer's Blog on Machine Learning"
      url: "https://www.brandonrohrer.com/blog.html"
      info: "Excellent resource for practical machine learning concepts explained with clarity. Brandon's writing breaks down complex topics into accessible explanations with real-world applications and insights."
    
    - type: id_rr
      title: "Papers With Code"
      url: "https://paperswithcode.com/"
      info: "Essential resource for staying current with AI research. This platform links academic papers with their code implementations, making it easier to understand and apply cutting-edge techniques in computer vision and machine learning."
    
    - type: id_rr
      title: "Distill: Machine Learning Research"
      url: "https://distill.pub/"
      info: "Exceptional publication featuring clear, interactive explanations of complex machine learning concepts. Their visual approach to explaining neural networks and other AI systems has significantly influenced my understanding of these technologies."
    
    - type: id_rr
      title: "Samsung Developer Documentation"
      url: "https://developer.samsung.com/"
      info: "Comprehensive resource for Samsung platform development, including Samsung Health SDK, Bixby, and SmartThings. Essential reference for anyone working on Samsung ecosystem integration."
    
    - type: id_rr
      title: "TensorFlow Documentation"
      url: "https://www.tensorflow.org/guide"
      info: "Definitive guide to TensorFlow development, covering everything from basic concepts to advanced model deployment. Particularly useful for understanding model optimization for edge devices."
---
