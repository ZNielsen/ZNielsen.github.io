---
layout: page
title: Sticker Blog
permalink: /blog/stickers
---

This is my collection of stickers!

For the longest time I did not want to sully anything I owned by slapping stickers all over it.  I do not like the aesthetic when it comes to cars, laptops, books, phones, etc., so I ended up just collecting stickers without doing anything with them.  Eventually, I hit a critical mass of stickers where I figured it would look good on something; one sticker is an advertisement, but a bunch of stickers is a collection.  I decided to put all my stickers on the water bottle I use at work.  It's gotten to the point where any sticker I place is covering others up, so I decided to start this catalog of stickers so I don't forget any that have been completely covered.

{% assign items = site.stickers | reverse %}
{% for sticker in items %}
- [Sticker: {{ sticker.title }}]({{ sticker.url }})
{% endfor %}

subscribe to only stickers [via RSS](https://zachn.me/feed/stickers.xml)
