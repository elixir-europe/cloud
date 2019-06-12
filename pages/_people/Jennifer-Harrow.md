---
title: "Jennifer Harrow"
layout: default
image_file: "jharrow.jpg"
excerpt_separator: <!--more-->
category:
  - contact
  - people
tags:
  - contacts
  - people
---

{% for static_file in site.static_files %}
  {% if static_file.path contains page.image_file %}
<img style="float: right; width: 80px;" src="{{ static_file.path | relative_url}}" />
  {% endif %}
{% endfor %}

## {{ page.title }}, PhD

ELIXIR Tools Platform Coordinator  
ELIXIR Hub  

<!--more-->

email [jennifer.harrow@elixir-europe.org](mailto:jonathan.tedds@elixir-europe.org)  


