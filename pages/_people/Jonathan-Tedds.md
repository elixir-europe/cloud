---
title: "Jonathan Tedds"
layout: default
image_file: "jtedds.jpg"
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

ELIXIR Compute Platform Coordinator  
ELIXIR Hub  

<!--more-->

email [jonathan.tedds@elixir-europe.org](mailto:jonathan.tedds@elixir-europe.org)  
web [Linkedin](https://uk.linkedin.com/in/jtedds)


