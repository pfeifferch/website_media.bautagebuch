---
layout: default
permalink: /category/bautagebuch/index.html 
title: Kategorie Bautagebuch
---

{% for post in site.posts %}

<ul class="clear">
<li class="date-meta">
<div class="genericon genericon-month"></div>
<span class="screen-reader-text">date</span>
<a href="{{ post.url }}" rel="bookmark" title="{{ post.date | date_to_string }}">{{ post.date | date_to_string }}</a>
</li>
</ul>

{% endfor %}
