---
layout: home
title: Home
permalink: index.html
nav_order: 1
---

# Software Engineering Immersive

**Today's topics** are on the [calendar]({% link calendar.md %}), along with links to **course material**, **resources**, and **lab assignments**.



## ✨ What's up today
{: .pt-3 .home-posts-headline }

{% assign daily_posts = site.daily_posts | reverse %}
{% for post in daily_posts %}
{{ post }}
{% endfor %}
