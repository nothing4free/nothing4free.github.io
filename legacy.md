---
layout: page
title: "/legacy"
permalink: /legacy
---

### welcome to /legacy. here you will find the old nothing4free.org blog posts and content.<br>

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: '%d %B %Y' }}
    </li>
  {% endfor %}
</ul>