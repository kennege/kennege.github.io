---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

You can also find my articles on my <u><a href="https://scholar.google.com/citations?user=YXhev9oAAAAJ&hl=en">Google Scholar profile</a>.</u>

{% include base_path %}

{% for post in site.publications reversed %}
  {% include publication.html %}
{% endfor %}

