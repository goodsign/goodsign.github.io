---
layout: page
title: Последние события
tagline: Supporting tagline
---

<ul class="posts">
  {% for post in site.posts offset: 0 limit: 10 %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

[Архив сообщений](/archive.html)