---
layout: default
permalink: /category/bautagebuch/index.html 
title: Kategorie Bautagebuch
---

{% for post in site.categories.Bautagebuch %} 
<blockquote>
<svg class="genericons genericons-{{ post.layout }}" width="16px" height="16px"><use xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="genericons-neue.svg#{{ post.layout }}"></use></svg>
<span class="screen-reader-text">{{ post.title }}</span>
<h2 class="entry-title">
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
