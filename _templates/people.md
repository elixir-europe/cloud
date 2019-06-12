---
title: "Joe Bloggs"
layout: default
date: 1967-11-11
excerpt_separator: <!--more-->
excerpt_link: # an optional link to different page when clicking the excerpt
www_link: # a simple web address related to the post, e.g. https://www.ga4gh.org
www_links_formatted:  # one or multiple complete links
#  - '<a href="https://www.biorxiv.org" target="_blank">[biorXiv]</a>'
image_file: 'login.png'
category:
  - people
tags: # please delete unneeded options
  - contacts
  - contributors
  - developers
---

{% for static_file in site.static_files %}
  {% if static_file.path contains page.image_file %}
<img style="float: right; max-width: 80px;" src="{{ static_file.path | relative_url}}" />
  {% endif %}
{% endfor %}

## {{ page.title }}

Person Role  

* email [person@example.com](mailto:person@example.com)  
* web [website](https://example.com/person)  

<!--more-->

Ion Tichy is a character in the works of Stanislaw Lem.





