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
    header: "Publications"
    info: "And Education, Skills, Certifications & Miscellaneous Information."

  # To change order of the Categories, simply change order. (you don't need to change list order.)
  category:
    - title: "Resume"
      type: id_resume
      color: "green"
    - title: "Publications & Press"
      type: id_pub
      color: "#F4A273"
    - title: "Media"
      type: id_media
      color: "#14A273"
    - title: "Education"
      type: id_edu
      color: "orange"
    - title: "Relevant Skills"
      type: id_skills
      color: "yellow"
    - title: "Certifications"
      type: id_cert
      color: "blue"
    - title: "Recommended Reads"
      type: id_rr
      color: "gray"

    # - title: "Programming"
    #   type: id_programming
    #   color: "#62b462"

  list:
    - type: id_resume
      title: "Udit Jain Resume"
      url: "https://drive.google.com/file/d/1hp81IaoKNDYjjmG2tCerTp56EoJQgVad/view?usp=sharing"
      info: "This is my brief Resume as of 2024."
    
    - type: id_pub
      title: "ArXiv"
      url: "https://arxiv.org/abs/1910.01642"
      info: "APEX: Adaptive Ext4 File System for Enhanced Data Recoverability in Edge Devices. Paper co-authored and published in: Proceedings of the 11th IEEE International Conference on Cloud Computing, Sydney, Australia, 2019"
    
    - type: id_pub
      title: "ArXiv"
      url: "https://arxiv.org/abs/1911.01941"
      info: "Transformative effects of IoT, Blockchain and Artificial Intelligence on cloud computing: Evolution,vision, trends and open challenges. Paper co-authored and published in: Distributed, Parallel, and Cluster Computing (cs.DC) 2019"
    
    - type: id_pub
      title: "Two color Disjunctive Rado Number "
      url: ""
      info: "(Under Review) Two color Disjunctive Rado Number for system of linear equations. Developed the algorithm for coloring equations with numbers to solve the system of equations."
    
    - type: id_pub
      title: "Professor Shibata's Blog"
      url: "https://tom-shibata.hatenablog.com/entry/2018/06/16/073923"
      info: "Elderly Clothing Assistance BAXTER robot was displayed in the RoboMech 2018 and 2019 and also the iREX 2019 exhibition. Coverage on Japanese National Television."

    - type: id_media
      title: "Samsung Smart Refrigerator"
      url: "https://www.youtube.com/watch?v=239uUZCIuqU"
      info: "Samsung's Smart Refrigerator, AI Inside, Developer Story"

    - type: id_media
      title: "Sleep with Pandemic"
      url: "https://news.samsung.com/global/understanding-sleep-how-our-sleeping-habits-changed-over-the-pandemic"
      info: "Insights on Global sleep changes before, during and after pandemic, Samsung Newsroom story."

    - type: id_media
      title: "Sleep with Pandemic, MBC"
      url: "https://www.youtube.com/watch?v=6yaVXXMIb6o"
      info: "Insights on Global sleep changes before, during and after pandemic, story covered by MBC news in Korea."

    - type: id_skills
      title: "Artificial Intelligence:"
      url: ""
      info: "Deep Learning, Computer Vision, TensorFlow, Keras, PyTorch, TensorFlow Lite, OpenCV, Natural Language Processing (NLP): SpaCy, KlonPY, NLTK, OpenIE, StanfordIE, Data Analytics: Semantic Information Extraction, Post-Processing Heuristics. Monte Carlo Simulation, Inverse Rendering, GPU Acceleration, NPU-toolkit (vsi-acuity)"
    
    - type: id_skills
      title: "Robotics & Automation:"
      url: ""
      info: "ROS (Robot Operating System), Baxter Robot, Robotic Manipulation, Robotics AI Integration: Combining AI and robotics for practical applications, Robotic Systems Design"
    
    - type: id_skills
      title: "Development:"
      url: ""
      info: "Programming Languages: C, C++, Java, Kotlin, Python, Matlab, SQL, Frameworks & Libraries: OpenCV, CUDA, OpenMP, MPI, SK-learn, Software Architecture: Clean Architecture Design Principles, Systems Design and Programming, Cloud Computing: AWS Cloud Deployment, S3, EMR, AWS Big Data Solutions, Database Management: SQL, AWS Athena, Google BigQuery, Room DB, Data Visualization: Apache Superset"
    
    # - type: id_skills
    #   title: "Robotics & Automation:"
    #   url: ""
    #   info: ""
    
    # - type: id_skills
    #   title: "Robotics & Automation:"
    #   url: ""
    #   info: ""
    

# Software skills
# Languages Java, C, C++, Assembly, Python, Ocaml, Matlab, VHDL, Prolog, Javascript, C#, UML, LaTex, R
# Libraries Spacy, NTLK, OpenIE, StanfordIE, KlonPy, LibFUSE, SATsovler, MiniNet, OpenCV, OpenGL, Tensorflow,
# Keras, PyTorch, Bash Scripting, Django, FogBus, Doxygen
# Softwares QEMU, Arduino Programming, Linux, Vivado Design Suite , Xilinx ISE, FPGA programming, Unity 3D game
# studio, Android Programming, Autodesk Inventor (CAD)
# Udit Jain
# Education
# 2016–2020 Computer Science and Engineering, Indian Institute of Technology, Delhi, CGPA – 9.10 .
# 2014–2016 Senior Secondary Education, St. Kabir Modern School, Delhi, Percentage – 94.2%.
# Till 2014 Secondary Education, St. Lawrence Convent Senior Secondary School, Delhi, CGPA – 9.8 
    # jekyiiliquid
    - type: id_rr
      title: "Brandon's Blog"
      url: "https://www.brandonrohrer.com/blog.html"
      info: "Interesting read across a variety of subjects."
    # - type: id_jekyiiliquid
    #   title: "Jekyll Cheat Sheet"
    #   url: "https://cloudcannon.com/community/jekyll-cheat-sheet/"
    #   info: "There are so many Jekyll variables and filters to remember and it can be tricky to keep it all in your head. This cheat sheet serves as a quick reference of everything Jekyll can do."
    # - type: id_jekyiiliquid
    #   title: "Liquid for Designers"
    #   url: "https://github.com/Shopify/liquid/wiki/Liquid-for-Designers"
    #   info: "Liquid for Designers wiki on GitHub."
    # - type: id_jekyiiliquid
    #   title: "Liquid for Programmers"
    #   url: "https://github.com/Shopify/liquid/wiki/Liquid-for-Programmers"
    #   info: "Liquid for Programmers wiki on GitHub."
    # - type: id_jekyiiliquid
    #   title: "Liquid Reference"
    #   url: "https://shopify.dev/api/liquid/"
    #   info: "Liquid is a template language created by Shopify and written in Ruby. It is now available as an open source project on GitHub."

    # # webdesign
    # - type: id_webdesign
    #   title: "W3Schools"
    #   url: "https://www.w3schools.com/"
    #   info: "W3Schools offers free online tutorials, references and exercises in all the major languages of the web. Covering popular subjects like HTML, CSS, JavaScript, Python, SQL, Java, and many more."
---
