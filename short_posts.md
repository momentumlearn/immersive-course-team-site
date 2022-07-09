---
layout: page
title: Short Posts
description: A feed containing all of the occasional short posts
nav_order: 6
---

# News Flashes

short_posts are stored in the `_short_posts` directory and rendered according to the layout file, `_layouts/short_posts.html`.

{% assign short_posts = site.short_posts | reverse %}
{% for post in short_posts %}
{{ post }}
{% endfor %}
