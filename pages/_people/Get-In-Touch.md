---
title: "Getting in touch"
layout: default
image_file: "getintouch.jpg"
excerpt_separator: <!--more-->
category:
  - contact
tags:
  - contacts
  - .featured
---

{% for static_file in site.static_files %}
  {% if static_file.path contains page.image_file %}
<img style="float: right; width: 80px;" src="{{ static_file.path | relative_url}}" />
  {% endif %}
{% endfor %}

## Getting in touch

We invite anyone from ELIXIR Nodes interested in these standards and/or the systems that implement them to join us on these calls.
- [Bi-weekly Calls](http://bit.ly/elixir-cloud-zoom) Every alternate Wednesday 10:00 - 11:00 GMT(London)

- [Meeting Agenda and Notes](http://bit.ly/elixir-cloud-minutes)

- [Slack](https://join.slack.com/t/elixir-cloud/shared_invite/enQtNzA3NTQ5Mzg2NjQ3LTZjZGI1OGQ5ZTRiOTRkY2ExMGUxNmQyODAxMDdjM2EyZDQ1YWM0ZGFjOTJhNzg5NjE0YmJiZTZhZDVhOWE4MWM) for real-time conversations, keep decisions and important info in GitHub issues please.

- [Mailing List](https://elixir-europe.org/intranet/cloud) for discussion and meeting announcements.
