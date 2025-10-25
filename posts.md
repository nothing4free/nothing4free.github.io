---
layout: page
title: "/posts"
permalink: /posts
---

# /posts

Writeups, artículos, lo que se me pase por la cabeza y documente por escrito :)

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: '%B %d %Y' }}
    </li>
  {% endfor %}
</ul>
