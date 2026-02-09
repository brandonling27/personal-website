---
layout: default
title: Home
---

<nav>
  <ul>
    <li><a href="/personal-website/">Home</a></li>
    <li><a href="/personal-website/blog/">Blog</a></li>
    <li><a href="/personal-website/about/">About</a></li>
  </ul>
</nav>

# Welcome to Brandon Ling's Personal Website

Hi! I'm Brandon Ling, and this is my personal space on the web.

## What I Do

I'm passionate about technology, software development, and continuous learning. This website serves as a place to share my thoughts, projects, and experiences.

## Latest Posts

<ul>
  {% for post in site.posts limit:5 %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span>
    </li>
  {% endfor %}
</ul>

[View all posts →](/personal-website/blog/)

## Quick Links

- [About Me](/personal-website/about/) - Learn more about who I am
- [Blog](/personal-website/blog/) - Read my latest thoughts and articles
- [GitHub](https://github.com/brandonling27) - Check out my code

---

_Thanks for visiting!_
