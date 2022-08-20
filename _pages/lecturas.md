---
layout: default
permalink: /lecturas/
title: "Reading Lists"
---

<br>
These are some of my on-going reading lists.

{% if page.url contains page.title %}
{% else %}
    <div class="mb3">
        These are some of my on-going reading lists:
    </div>
{% endif %}


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
        {{ post.excerpt }}
    </time> 
    </div>
{% endfor %}
<br>
</div>
