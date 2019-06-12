---
title: "Alexander Kanitz"
layout: default
image_file: "akanitz.jpg"
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

Technical Product Lead (WES-ELIXIR)  
Technical Product Co-Lead (Web Portal)  
ELIXIR-CH, University of Basel  

<!--more-->

email [alexander.kanitz@unibas.ch](mailto:alexander.kanitz@unibas.ch)  
web [ResearchGate](https://www.researchgate.net/profile/Alexander_Kanitz)


