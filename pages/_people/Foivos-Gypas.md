---
title: "Foivos Gypas"
layout: default
image_file: "fgypas.jpg"
excerpt_separator: <!--more-->
categories:
  - people
tags:
  - people
  - developers
---

{% for static_file in site.static_files %}
  {% if static_file.path contains page.image_file %}
<img style="float: right; width: 80px;" src="{{ static_file.path | relative_url}}" />
  {% endif %}
{% endfor %}

## {{ page.title }}, PhD

University of Basel  
ELIXIR-CH

<!--more-->

email [alexander.kanitz@unibas.ch](mailto:alexander.kanitz@unibas.ch)  
web [ResearchGate](https://www.researchgate.net/profile/Alexander_Kanitz)


