---
title: "Marius Dieckmann"
layout: default
image_file: "mdieckmann.jpg"
excerpt_separator: <!--more-->
categories:
  - people
tags:
  - people
  - developers
---

{% for static_file in site.static_files %}
  {% if static_file.path contains page.image_file %}
<img style="float: right; width: 65px;" src="{{ static_file.path | relative_url}}" />
  {% endif %}
{% endfor %}

## {{ page.title }}

Technical Product Co-Lead (Web Portal)  
ELIXIR-DE, University of Giessen  

<!--more-->

email [marius.dieckmann@computational.bio.uni-giessen.de](mailto:marius.dieckmann@computational.bio.uni-giessen.de)  
web [Uni-Geissen](https://www.uni-giessen.de/fbz/fb08/Inst/bioinformatik/people/researchassistants/marius_dieckmann)


