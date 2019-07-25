---
title: "Yasset Perez Riverol"
layout: default
image_file: "yperez.jpg"
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

Technical Product Lead (Biocontainers)  
EMBL-EBI  

<!--more-->

email [yperez@ebi.ac.uk](mailto:yperez@ebi.ac.uk)  
web [EMBL-EBI](https://www.ebi.ac.uk/about/people/yasset-perez-riverol)


