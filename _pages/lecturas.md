---
layout: page
permalink: /lecturas/
title:
---

<h1 class="f2 lh-title">Reading Lists</h1>

![iago](https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fsucedioenoaxaca.com%2Fwp-content%2Fuploads%2F2016%2F12%2Fbioiago-1050x700.jpg&f=1&nofb=1)

Here is a collection of thematic lists that I use to keep track of the books I read for pleasure (mostly literature).

<div class="fl w-100">
{% for post in site.categories.lecturas %}
    <time class="di-ns f6 ttu tracked gray code">
        {{ post.date | date_to_string }}
    </time>

    <div class="di-ns mb2">
    <a class="link black hover-red" href="{{ BASE_PATH }}{{ post.url }}">
        {{ post.title }}
    </a><br>
    </div>
{% endfor %}
</div>
