---
layout: default
title: Digital Projects Studio
---
{% assign skip = "debate_analysis|clarkdatalabs.github.io" | split: '|'  %}
{% assign workshop = "mapping_R|datavis_r" | split: '|'  %}
Welcome to the Digital Projects Studio's Github Page
{% for repository in site.github.public_repositories %}
 {% unless skip contains repository.name or workshop contains repository.name%}
  * [{{ repository.name }}](http://clarkdatalabs.github.io/{{ repository.name }})
 {% endunless %}
{% endfor %}

Workshops

{% for repository in workshop %}
 * [{{ repository }}](http://clarkdatalabs.github.io/{{ repository }})
{% endfor %}
