---
title: "Susheel Varma"
layout: default
image_file: "svarma.jpg"
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

ELIXIR Project Champion (Cloud)  
ELIXIR Compute Platform Task 4 Lead  
GA4GH TRS / TES Standard Co-lead  
EMBL-EBI  

<!--more-->

email [susheel.varma@ebi.ac.uk](mailto:susheel.varma@ebi.ac.uk)  
web [EMBL-EBI](https://www.ebi.ac.uk/about/people/susheel-varma)


