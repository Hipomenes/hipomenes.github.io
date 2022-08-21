---
layout: page
permalink: /lecturas/
title:
---

<h1 class="f2 lh-title">Reading Lists</h1>

<br>

Here is a collection of the reading lists that I use to keep track of the books I read for pleasure (mostly literature.

<br>
<div class="fl w-100">
{% for post in site.categories.lecturas %}
    <time class="di-ns f6 ttu tracked gray code">
        {{ post.date | date_to_string }}
    </time>

    <div class="di-ns mb2">
    <a class="link black bold hover-red" href="{{ BASE_PATH }}{{ post.url }}">
        {{ post.title }}
    </a>
        <time class="fw8-m grey">
    </time> 
    </div>
{% endfor %}
<br>
<br>
</div>
