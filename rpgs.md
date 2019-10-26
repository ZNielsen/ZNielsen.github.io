---
layout: page
title: RPG Log Blog
permalink: /blog/rpgs
---

I enjoy playing and running RPGs.  About to get into Numenera, currently running Lady Blackbird


{% assign items = site.rpgs | sort: 'date' %}
{% for log in items %}
- [Sticker: {{ log.name }}]({{ log.url }})
{% endfor %}
