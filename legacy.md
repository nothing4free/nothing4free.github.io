---
layout: page
title: "/legacy"
permalink: /legacy
---

### welcome to /legacy. here you will find the old nothing4free.org blog posts and content.

{% for post in site.posts %}
- [post.url]({{ post.title }}) - {{ post.date | date: '%Y-%m-%d' }}
{% endfor %}