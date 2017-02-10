---
title: Code
layout: default
---
{% for item in site.categories.code reversed %}
[{{ item.title }}]({% if item.external_url %}{{ item.external_url }}{% else %}{{ item.url }}{% endif %})
{% if item.description %} -- {{ item.description }}{% endif %}
{% endfor %}
