---
layout: post
title:  "Gallery"
date:   2022-03-27 12:13:49 +0100
categories: jekyll update
---

<!-- 
![](/photos/1.jpeg)

![](/photos/2.jpeg)

![](/photos/3.jpeg) 
-->

{% for image in site.static_files %}
 {% if image.path contains 'photos/' %}
  ![image]({{ image.path }} 'image')
 {% endif %}
{% endfor %}