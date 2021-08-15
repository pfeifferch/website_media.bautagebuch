---
layout: default
permalink: /author/index.html 
title: Autoren
---
{% for page in site.pages %}
{% if page.categories contains 'Authors' %}

<blockquote>
<span class="screen-reader-text">{{ post.title }}</span>
<h2 class="entry-title">
<a href="{{ post.url }}" rel="bookmark">{{ post.title }}</a>
</h2>
<h5 class="entry-date">
<a href="{{ post.url }}" title="{{ post.title }}" rel="bookmark">
<time class="entry-date" datetime="{{ post.date | date_to_string }}" pubdate>{{ post.date | date_to_string }} </time>
</a>
</h5>
</blockquote>

{% endif %}
{% endfor %}
