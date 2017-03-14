---
title: Notes
layout: default
---
Instead of a blog, I like the idea of an ongoing collection of notes on various
topics.

{% for item in site.categories.notes %}
[{{ item.title }}]({{ item.url }})
{% endfor %}
