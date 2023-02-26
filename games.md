---
layout: page
title: Game Log
permalink: /blog/games
---

I enjoy playing boardgames and RPGs.

{% assign items = site.games | reverse %}
{% for log in items %}
- [{{ log.playdate | date: "%Y.%m.%d" }} — {{ log.name }}]({{ log.url }})
{% endfor %}

subscribe to only games [via RSS](https://zachn.me/feed/games.xml)
