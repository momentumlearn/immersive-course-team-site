---
layout: page
title: TODOs
description: A feed containing all of the daily posts
nav_order: 6
---

# Daily Posts

daily_posts are stored in the `_daily_posts` directory and rendered according to the layout file, `_layouts/daily_posts.html`.

{% assign daily_posts = site.daily_posts | reverse %}
{% for post in daily_posts %}
{{ post }}
{% endfor %}
