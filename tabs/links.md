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
    header: "Links"
    info: "Your Links page description."

  # To change order of the Categories, simply change order. (you don't need to change list order.)
  category:
    - title: "Resume"
      type: id_resume
      color: "green"
    - title: "Publications"
      type: id_pub
      color: "#F4A273"
    - title: "Press"
      type: id_press
      color: "#14A273"
    - title: "Education"
      type: id_edu
      color: "orange"
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
    
    - type: id_press
      title: "Professor Shibata's Blog"
      url: "https://tom-shibata.hatenablog.com/entry/2018/06/16/073923"
      info: "Elderly Clothing Assistance BAXTER robot was displayed in the RoboMech 2018 and 2019 and also the iREX 2019 exhibition. Coverage on Japanese National Television."


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
