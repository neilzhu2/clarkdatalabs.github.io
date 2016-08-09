---
layout: default
title: Digital Projects Studio
---
{% assign skip = "debate_analysis|clarkdatalabs.github.io" | split: '|'  %}
Welcome to the Digital Projects Studio's Github Page
{% for repository in site.github.public_repositories %}
 {% unless skip contains repository.name %}
  * {{ repository.name }}
 {% endunless %}
{% endfor %}
