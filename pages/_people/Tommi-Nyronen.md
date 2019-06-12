---
title: "Tommi Nyrönen"
layout: default
image_file: "tnyronen.jpg"
excerpt_separator: <!--more-->
categories:
  - people
tags:
  - people
---

{% for static_file in site.static_files %}
  {% if static_file.path contains page.image_file %}
<img style="float: right; width: 80px;" src="{{ static_file.path | relative_url}}" />
  {% endif %}
{% endfor %}

## {{ page.title }}, PhD

ELIXIR-FI Head of Node  
ELIXIR Compute Platform ExCo  
ELIXIR-FI - CSC  

<!--more-->

email [tommi.nyronen@csc.fi](mailto:tommi.nyronen@csc.fi)  
web [Linkedin](https://www.linkedin.com/in/nyronen)


