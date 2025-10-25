---
layout: page
title: "/writeups"
permalink: /writeups
---

# /writeups

Una colección de writeups de CTF (principalmente, Hack the Box) y otros desafíos varios.

<ul>
  {% for post in site.writeups %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: '%B %d %Y' }}
    </li>
  {% endfor %}
</ul>