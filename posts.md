---
layout: default
permalink: /category/bautagebuch/index.html 
title: Kategorie Bautagebuch
---

{% for post in site.posts %}

<article id="{{ post.title }}" class="post-content {{ post.title }} post type-post status-publish format-standard hentry category-bautagebuch">
<a href="{{ post.url }}" rel="bookmark">{{ post.title }}</a>
<header class="entry-header">
<span class="screen-reader-text">{{ post.title }}</span>
<h2 class="entry-title">
<a href="{{ post.url }}" rel="bookmark"></a>
</h2>
<div class="entry-meta">
  <h5 class="entry-date">
  <a href="{{ post.url }}" title="{{ post.title }}" rel="bookmark">
  <time class="entry-date" datetime="{{ post.date | date_to_string }}" pubdate>{{ post.date | date_to_string }} </time></a>
  <span class="byline"></span>
  </h5>
</div>
</article>
{% endfor %}
