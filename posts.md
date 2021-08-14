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
<a href="{{ post.url }}" rel="bookmark">{{ post.title }}</a>
</h2>
<div class="entry-meta">
<h5 class="entry-date">
<!--
By <span class="author vcard">
<a class="url fn n" href="./../../author/chris/index.html" title="View all posts by Chris" rel="author">Chris</a></span> | 
-->
<a href="{{ post.url }}" title="{{ post.title }}" rel="bookmark">
<time class="entry-date" datetime="{{ post.date | date_to_string }}" pubdate>{{ post.date | date_to_string }} </time></a><span class="byline">
<span class="sep"></span>
 | <span class="screen-reader-text">Comments </span> <a href="./../../bautagebuch/erdarbeiten-tag-5/index.html#respond" class="comments-link">0 Comment</a>
</span>
</h5>
</div>
{% endfor %}
