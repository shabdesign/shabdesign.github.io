---
layout: blog
title: Blog
nav: true
footer: true
description: My Blog Section
permalink: /blog/
---

# Blog

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span> – {{ post.date | date: "%B %d, %Y" }}</span>
    </li>
  {% endfor %}
</ul>
