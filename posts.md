---
layout: default
permalink: /category/bautagebuch/index.html 
title: Kategorie Bautagebuch
---

{% for post in site.categories.Bautagebuch %} 
<blockquote>
<span class="screen-reader-text">{{ post.title }}</span>
<h2 class="entry-title genericon genericon-{{ post.layout }}">
<a href="{{ post.url }}" rel="bookmark">{{ post.title }}</a>
</h2>
<h5 class="entry-date">
<a href="{{ post.url }}" title="{{ post.title }}" rel="bookmark">
<time class="entry-date" datetime="{{ post.date | date_to_string }}" pubdate>{{ post.date | date_to_string }} </time>
</a>
{{ post.excerpt }}
</h5>
</blockquote>

{% endfor %}
