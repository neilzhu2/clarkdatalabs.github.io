---
layout: default
title: Digital Projects Studio
---

{% assign skip = "debate_analysis|clarkdatalabs.github.io" | split: '|'  %}
{% assign workshop = "mapping_R|datavis_r" | split: '|'  %}

# Welcome to the Digital Projects Studio's Github Page

The Digital Projects Studio is part of the University of Michigan's Clark Library and provides tutorials and support for visualization work. Connect to our workshops and projects below, and to our blog an additional information [here](https://digitalprojectstudio.wordpress.com/).

## Workshops

{% for repository in workshop %}
 * [{{ repository }}](http://clarkdatalabs.github.io/{{ repository }})
{% endfor %}

## Projects

{% for repository in site.github.public_repositories %}
 {% unless skip contains repository.name or workshop contains repository.name%}
  * [{{ repository.name }}](http://clarkdatalabs.github.io/{{ repository.name }})
 {% endunless %}
{% endfor %}


