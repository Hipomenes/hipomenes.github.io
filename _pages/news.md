---
layout: default
permalink: /news/
title: "news"
---

<br>
See some of my recent activities:

{% if page.url contains page.title %}
{% else %}
    <div class="mb3">
        Read some of my recent notes here:
    </div>
{% endif %}


<div class="fl w-100">
{% for post in site.categories.news %}
    <time class="di-ns f6 ttu tracked gray code">
        {{ post.date | date_to_string }}
    </time>

<div class="di-ns mb2">
    <a class="link black fw6 hover-washed-red hover-underline" href="{{ BASE_PATH }}{{ post.url }}">
        {{ post.title }}
    </a>
        <time class="fw8-m grey">
        {{ post.excerpt }}
    </time> 
    </div>
    
{% endfor %}
<br>
</div>

