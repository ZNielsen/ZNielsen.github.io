---
layout: page
title: RPG Log Blog
permalink: /blog/rpgs
---

I enjoy playing and running RPGs.  About to get into Numenera, currently running Lady Blackbird


{% assign items = site.rpg | sort: 'date' %}
{% for log in items %}
- [{{ log.playdate }}: {{ log.name }}]({{ log.url }})
{% endfor %}
