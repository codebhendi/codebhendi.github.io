---
layout: default
title: Home
---

# Welcome to Shubham's Blog

I write about frontend development, UI systems, and my journey working with modern frameworks like React and Svelte.

## Latest Posts

{% for post in site.posts %}
  - [{{ post.title }}]({{ post.url }}) — *{{ post.date | date: "%B %d, %Y" }}*
{% endfor %}

## Pages

- [Career Journey](/career/)

---

*Bookmark this to keep an eye on my project updates.*
