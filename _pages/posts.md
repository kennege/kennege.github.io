---
layout: archive
title: "Posts"
permalink: /posts/
author_profile: true
redirect_from: 
  - /posts
  - /posts.md
---


{% include base_path %}

{% for post in site.research reversed %}
  {% include publication.html %}
{% endfor %}

