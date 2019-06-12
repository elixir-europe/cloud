---
title: "Ilkka Lappalainen"
layout: default
image_file: "ilappalainen.jpg"
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

ELIXIR Human Data  
ELIXIR-GA4GH Strategic Partnership  
ELIXIR-FI - CSC

<!--more-->

email [ilkka.lappalainen@csc.fi](mailto:ilkka.lappalainen@csc.fi)

