---
title: "Ania Niewielska"
layout: default
image_file: "aniewielska.jpg"
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

## {{ page.title }}

Technical Product Lead (TESK)  
EMBL-EBI  

<!--more-->

email [aniewielska@ebi.ac.uk](mailto:aniewielska@ebi.ac.uk)  
web [EMBL-EBI](https://www.ebi.ac.uk/about/people/ania-niewielska)


