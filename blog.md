---
layout: default
title: Blog
permalink: /blog/
---

<nav>
  <ul>
    <li><a href="/me/">Home</a></li>
    <li><a href="/me/blog/">Blog</a></li>
    <li><a href="/me/about/">About</a></li>
  </ul>
</nav>

# Blog

Welcome to my blog! Here I share my thoughts, learnings, and experiences on various topics related to software development, technology, and more.

---

{% for post in site.posts %}
## [{{ post.title }}]({{ post.url | relative_url }})

**{{ post.date | date: "%B %d, %Y" }}**

{{ post.excerpt }}

[Read more →]({{ post.url | relative_url }})

---

{% endfor %}

{% if site.posts.size == 0 %}
_No posts yet. Check back soon!_
{% endif %}
