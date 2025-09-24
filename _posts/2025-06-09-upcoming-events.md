---
layout: post
title: Upcoming Events
date: 2025-06-09 21:48
category: listing
author: Aisling
tags: []
summary: 
---

{% for post in site.posts %}
    {% if post.tags contains 'upcoming_events' %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
    {% endif %}
{% endfor %}