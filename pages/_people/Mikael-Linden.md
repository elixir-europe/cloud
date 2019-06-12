---
title: "Mikael Linden"
layout: default
image_file: "mlinden.jpg"
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

## {{ page.title }}, PhD

ELIXIR Project Champion (AAI)  
ELIXIR Compute Platform Task 1 Lead  
ELIXIR-FI, CSC  

<!--more-->

email [mikael.linden@csc.fi](mailto:mikael.linden@csc.fi)  
