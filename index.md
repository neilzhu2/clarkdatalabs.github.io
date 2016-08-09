---
layout: default
title: Digital Projects Studio
---
{% assign skip = ['debate_analysis'] %}
Welcome to the Digital Projects Studio's Github Page
{% for repository in site.github.public_repositories %}
 {% if skip contains repository.name %}
  * {{ repository.name }}
 {% endif %}
{% endfor %}
