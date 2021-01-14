---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  You can also find my articles on <a href="{{site.author.googlescholar}}" target="_blank"><u>my Google Scholar profile</u></a>.
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include publication.html %}
{% endfor %}
