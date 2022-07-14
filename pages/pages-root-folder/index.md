---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
header:
  image_fullwidth:
title: "CVMI Lab @ HKU"

#slider:
#text_color: white
#shadow_color: black
#slides: 
#  - image: gallery-example-1.jpg
#    slide_html:
#  - image: gallery-example-2.jpg
#    slide_html: "<h2>Yes, this carousel supports html texting</h2>"
#  - image: gallery-example-3.jpg
#    slide_html: "<h2>Yes, this carousel supports html texting</h2>"

sidebar: right

# widget1:
#   title: "GradNet ICCV2019 Demo"
#   url: 'https://youtu.be/tWDbs3VrnbU'
#   video: '<iframe width="360" height="240" src="https://www.youtube.com/embed/tWDbs3VrnbU" allow="accelerometer; encrypted-media; gyroscope; picture-in-picture" allowfullscreen style="max-width: 100%; max-height: 150pt;"></iframe>'
#   text: 'Check out our demo for Visual Object Tracking'
# widget2:
#   title: "Video Tracking"
#   url: 'https://www.youtube.com/watch?v=M1LqUV4jLbM'
#   text: 'Implementation of MDNet, KCF and SiamFC.'
#   video: '<iframe src="https://www.youtube.com/embed/M1LqUV4jLbM" width="360" height="240" allow="accelerometer; encrypted-media; gyroscope; picture-in-picture" allowfullscreen style="max-width: 100%; max-height: 150pt;"></iframe>'
# widget3:
#   title: "Pose Tracking"
#   url: 'https://youtu.be/CiKJuAH2U8I'
#   video: '<iframe src="https://www.youtube.com/embed/AL-8XCzRFo0" width="360" height="240" allow="accelerometer; encrypted-media; gyroscope; picture-in-picture" allowfullscreen style="max-width: 100%; max-height: 150pt;"></iframe>'
#   text: 'Our team won the 2nd place in the pose-track challenge.'

#
# Use the call for action to show a button on the frontpage
#
# To make internal links, just use a permalink like this
# url: /getting-started/
#
# To style the button in different colors, use no value
# to use the main color or success, alert or secondary.
# To change colors see sass/_01_settings_colors.scss
#
#callforaction:
#  url: https://tinyletter.com/feeling-responsive
#  text: Inform me about new updates and features ›
#  style: alert
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true

---


<div class="row main-content" style= "margin-top: 30px; max-height:540px; margin-left: 1%">
  <div class="column small-9 pc">
    
    <!-- carrousel -->

    <div id="myCarousel" class="carousel slide" data-ride="carousel" style="">
        <!-- Indicators -->
        <ol class="carousel-indicators">
          <li data-target="#myCarousel" data-slide-to="0" class="active"></li>
          <li data-target="#myCarousel" data-slide-to="1"></li>
          <li data-target="#myCarousel" data-slide-to="2"></li>
        </ol>

        <!-- Wrapper for slides -->
        <div class="carousel-inner">
          {% include carousel_item.html  active="true" 
             url="http://openaccess.thecvf.com/content_ICCV_2017/papers/Qi_3D_Graph_Neural_ICCV_2017_paper.pdf" 
             image="images/images_for_pub/3dgnn.png" 
             alt="3D Scene Understanding" 
             title="3D Scene Understanding" 
             caption="We aim at developing technologies for representation learning with 3D data (e.g. point clouds); RGB-D/3D semantic understanding (e.g. semantic segmentation, object detection, and instance segmentation) and registration  tasks." %}

          {% include carousel_item.html  
             url="http://openaccess.thecvf.com/content_cvpr_2018/papers/Qi_Semi-Parametric_Image_Synthesis_CVPR_2018_paper.pdf" 
             image="images/images_for_pub/data_efficient.png" 
             alt="Data-efficient Deep Learning" 
             title="Data-efficient and Computation-efficient Deep Learning" 
             caption="We are interested in developing computation-efficent deep learning algorithms and data-efficient deep learning methods including high-quality data synthesis methods, efficient image annotation systems, label-efficient learning strategies (e.g. self-supervised learning, weakly supervised learning, domain adaptation, and semi-supervised learning, etc)." %}

          {% include carousel_item.html  
             url="http://openaccess.thecvf.com/content_cvpr_2018/papers/Qi_GeoNet_Geometric_Neural_CVPR_2018_paper.pdf" 
             image="images/images_for_pub/high_quality_3d.png"
             alt="High-quality 3D Reconstruction" 
             title="High-quality 3D Reconstruction" 
             caption="We are dedicated to pushing the boundaries of 3D sensing with learning-based approaches, e.g. 3D object & scene reconstruction from a single image or videos; and sparse-to-dense or depth completion to enhance depth-sensing quality." %}
        </div>

        <!-- Left and right controls -->
        <a class="left carousel-control" href="#myCarousel" data-slide="prev">
          <span class="glyphicon glyphicon-chevron-left"></span>
          <span class="sr-only">Previous</span>
        </a>
        <a class="right carousel-control" href="#myCarousel" data-slide="next">
          <span class="glyphicon glyphicon-chevron-right"></span>
          <span class="sr-only">Next</span>
        </a>
    </div>
  </div>



  <!-- carrousel on mobile devices -->
  <div class="column small-12 mobile">
    
    <!-- carrousel -->

    <div id="myCarousel" class="carousel slide" data-ride="carousel" style="">
        <!-- Indicators -->
        <ol class="carousel-indicators">
          <li data-target="#myCarousel" data-slide-to="0" class="active"></li>
          <li data-target="#myCarousel" data-slide-to="1"></li>
          <li data-target="#myCarousel" data-slide-to="2"></li>
        </ol>

        <!-- Wrapper for slides -->
        <div class="carousel-inner">
          {% include carousel_item.html  active="true" 
             url="http://openaccess.thecvf.com/content_ICCV_2017/papers/Qi_3D_Graph_Neural_ICCV_2017_paper.pdf" 
             image="images/images_for_pub/3dgnn.png" 
             alt="3D Scene Understanding" 
             title="3D Scene Understanding" 
             caption="We aim at developing technologies for representation learning with 3D data (e.g. point clouds); RGB-D/3D semantic understanding (e.g. semantic segmentation, object detection, and instance segmentation) and registration  tasks." %}

          {% include carousel_item.html  
             url="http://openaccess.thecvf.com/content_cvpr_2018/papers/Qi_Semi-Parametric_Image_Synthesis_CVPR_2018_paper.pdf" 
             image="images/images_for_pub/data_efficient.png" 
             alt="Data-efficient Deep Learning" 
             title="Data-efficient and Computation-efficient Deep Learning" 
             caption="We are interested in developing computation-efficent deep learning algorithms and data-efficient deep learning methods including high-quality data synthesis methods, efficient image annotation systems, label-efficient learning strategies (e.g. self-supervised learning, weakly supervised learning, domain adaptation, and semi-supervised learning, etc)." %}

          {% include carousel_item.html  
             url="http://openaccess.thecvf.com/content_cvpr_2018/papers/Qi_GeoNet_Geometric_Neural_CVPR_2018_paper.pdf" 
             image="images/images_for_pub/high_quality_3d.png"
             alt="High-quality 3D Reconstruction" 
             title="High-quality 3D Reconstruction" 
             caption="We are dedicated to pushing the boundaries of 3D sensing with learning-based approaches, e.g. 3D object & scene reconstruction from a single image or videos; and sparse-to-dense or depth completion to enhance depth-sensing quality." %}
        </div>

        <!-- Left and right controls -->
        <a class="left carousel-control" href="#myCarousel" data-slide="prev">
          <span class="glyphicon glyphicon-chevron-left"></span>
          <span class="sr-only">Previous</span>
        </a>
        <a class="right carousel-control" href="#myCarousel" data-slide="next">
          <span class="glyphicon glyphicon-chevron-right"></span>
          <span class="sr-only">Next</span>
        </a>
    </div>
  </div>



  <div class="column small-3 pc" style="max-height: inherit">
  	<div><h3>News</h3></div>
    
    <div class="list-group" style="margin-left=0; max-height: inherit; overflow-y: auto;">
    {% include news_item.html 
        highlight="true" date="Always"
        content="We are hiring! Several Ph.D. positions are now available at HKU in computer vision and deep learning. Candidates with strong academic background and/or solid programming skills are highly preferred. Click <a href=\"recruitment\"><strong>here</strong></a> to see more details." %}
      
      {% include news_item.html  date="14-June-2022" content="Three papers are accepted to ECCV'22. Congratulations to my students and collaborators. Codes will be released soon!" %}
      
      {% include news_item.html  date="3-Mar-2022" content="Nine papers are accepted to CVPR'22. Proud of my students and collaborators. Thank all team members for providing support during the CVPR deadline. Codes will be released soon!" %}
     
    {% include news_item.html  date="20-Aug-2021" content="Two papers are accepted to ICCV'21 with one Oral." %}

    {% include news_item.html  date="20-Mar-2021" content="Five papers are accepted to CVPR'21 with two Orals." %}

    {% include news_item.html  date="27-Sep-2020" content="One paper is accepted to NeurIPS." %}

    {% include news_item.html  date="12-July-2020" content="One paper is accepted to TPAMI." %}

    {% include news_item.html  date="4-July-2020" content="Four papers are accepted to ECCV 2020 with one Oral (2%) and one Spotlight (5%)." %}

    
  		{% include news_item.html  date="1-Feb-2020" content="Our lab established!" %}


    </div>
  </div>
</div>

<div class="column small-12 mobile">
    <br>
    <h3>News</h3>
    <div class="list-group" style="margin-left=0; max-height: inherit; overflow-y: auto;">
      
    {% include news_item.html 
        highlight="true" date="Always"
        content="We are hiring! Several Ph.D. positions are now available at HKU in computer vision and deep learning. Candidates with strong academic background and/or solid programming skills are highly preferred. Click <a href=\"recruitment\"><strong>here</strong></a> to see more details." %}
   
       {% include news_item.html  date="14-June-2022" content="Three papers are accepted to ECCV'22. Congratulations to my students and collaborators. Codes will be released soon!" %}
      
      {% include news_item.html  date="3-Mar-2022" content="Nine papers are accepted to CVPR'22. Proud of my students and collaborators. Thank all team members for providing support during the CVPR deadline. Codes will be released soon!" %}
     
    {% include news_item.html  date="20-Aug-2021" content="Two papers are accepted to ICCV'21 with one Oral." %}

   {% include news_item.html  date="20-Mar-2021" content="Five papers are accepted to CVPR'21 with two Orals." %}

  {% include news_item.html  date="27-Sep-2020" content="One paper is accepted to NeurIPS." %}

    {% include news_item.html  date="12-July-2020" content="One paper is accepted to TPAMI." %}

    {% include news_item.html  date="4-July-2020" content="Four papers are accepted to ECCV 2020 with one Oral (2%) and one Spotlight (5%)." %}

    
      {% include news_item.html  date="1-Feb-2020" content="Our lab established!" %}


    </div>
    <h3 class="mobile"> Our Research </h3>
</div>


<div class="pc" style="margin-left: 2%">
<br>
<h3> Our Research </h3> 


</div>

---

<div class="pc" style="margin-left: 2%">
Our research aims at endowing machines with the capability to perceive, understand, and reconstruct the visual world with the following focuses: 
 <ul> 
  <li>developing scalable computation-efficient and label-efficient deep learning algorithms for natural and medical image analysis;</li>
  <li>designing effective techniques for 3D scene understanding and reconstruction;</li>
  <li>building lifelong learning machines that can learn continuously, transfer previous knowledge adn discover novel concepts (through interaction).</li>
 </ul>
</div>
