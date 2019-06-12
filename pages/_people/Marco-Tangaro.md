---
title: "Marco Tangaro"
layout: default
image_file: "mtangaro.png"
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

ELIXIR-IT, CNR  

<!--more-->

email [ma.tangaro@ibiom.cnr.it](mailto:ma.tangaro@ibiom.cnr.it)  


