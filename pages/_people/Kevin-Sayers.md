---
title: "Kevin Sayers"
layout: default
image_file: "ksayers.png"
excerpt_separator: <!--more-->
category:
  - contact
  - people
tags:
  - contacts
  - people
  - .featured
---

{% for static_file in site.static_files %}
  {% if static_file.path contains page.image_file %}
<img style="float: right; width: 80px;" src="{{ static_file.path | relative_url}}" />
  {% endif %}
{% endfor %}

## {{ page.title }}

ELIXIR Project Champion (Cloud)  
ELIXIR Compute Platform Task 4 Lead  
ELIXIR-CH - SPHN  

<!--more-->

email [kevin.sayers@unibas.ch](mailto:kevin.sayers@unibas.ch)  
web [Linkedin](https://www.linkedin.com/in/sayersk)


