---
layout: page
title: "/legacy"
permalink: /legacy
---
# /legacy
### welcome to /legacy. here you will find the old nothing4free.org blog posts and content.

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>