---
title: Et cetera
layout: default
---
## Art & Photography

{% assign items = site.photos | sort: "date" | reversed %}
{% for item in items %}
[{{ item.title }}](http://photos.paulwrankin.com{{ item.url }})
{% endfor %}

## Philosophy

[Being as an 'issue' for Dasein in Heidegger's fundamental ontology](http://files.paulwrankin.com/library/PHIL3300 Being as an issue for Dasein.pdf)
