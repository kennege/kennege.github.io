---
layout: archive
title: "Posts"
permalink: /posts/
author_profile: true
---


{% include base_path %}

{% for post in site.portfolio reversed %}
  {% include publication.html %}
{% endfor %}

