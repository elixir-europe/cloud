---
title: "People Template"
layout: default
date: 1967-11-11
excerpt_separator: <!--more-->
image_file: 'login.jpg'
category:
  - people
tags: # please delete unneeded options
  - contacts
  - contributors
  - developers
---

{% for static_file in site.static_files %}
  {% if static_file.path contains page.image_file %}
<img style="float: right; width: 80px;" src="{{ static_file.path | relative_url}}" />
  {% endif %}
{% endfor %}

## {{ page.title }}

Role
Organisation

email [person@example.com](mailto:persona@example.com)
web [Link](https://example.com)

<!--more-->

Ion Tichy is a character in the works of Stanislaw Lem.





