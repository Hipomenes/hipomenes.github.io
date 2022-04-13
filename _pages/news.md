---
layout: default
permalink: /news/
title: "news"
---

Recent activities

<ul>
  {% for post in site.categories.news %}
    {% if post.url %}
        <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>
