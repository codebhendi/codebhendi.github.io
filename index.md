---
layout: default
title: Shubham's Blog
---

# Frontend Engineering & UI Architecture

I write about building scalable UI systems, leading frontend teams, and the practical lessons learned navigating modern web development. My focus is on simplicity, maintainability, and pragmatic solutions over complexity.

## Latest Posts

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) — *{{ post.date | date: "%B %d, %Y" }}*
{% endfor %}

---

## About Me

**Frontend Engineer & Technical Lead** at Angel One  
Specializing in UI architecture, component systems, and leading teams through technology migrations.

[See my full career journey →](/career/)

