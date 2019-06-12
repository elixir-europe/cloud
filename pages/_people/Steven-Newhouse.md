---
title: "Steven Newhouse"
layout: default
image_file: "snewhouse.jpg"
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

ELIXIR Compute Platform ExCo  
Head of Technical Services Cluster, EMBL-EBI  
EMBL-EBI  

<!--more-->

email [steven.newhouse@ebi.ac.uk](mailto:steven.newhouse@ebi.ac.uk)  
web [EMBL-EBI](https://www.ebi.ac.uk/about/people/steven-newhouse)


