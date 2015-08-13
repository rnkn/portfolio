---
title: Mark Zuckerberg Fan-Fiction
layout: default
category: writing
---
I had a Facebook account in 2013. These are my collected status updates.
<!-- more -->
{% for item in site.categories.zuckerberg reversed %}
## {{ item.date | date: site.date_format }}
{{ item.content }}
{% endfor %}
