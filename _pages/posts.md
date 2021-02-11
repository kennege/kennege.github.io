---
layout: archive
title: "Posts"
permalink: /posts/
author_profile: true
---

A collection of posts about projects I have worked on in the past or that I find interesting.

{% include base_path %}

{% assign ordered_pages = site.research | sort:"order_number" %}

{% for post in ordered_pages %}
  {% include publication.html %}
{% endfor %}