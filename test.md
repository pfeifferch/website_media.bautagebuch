---
layout: default
permalink: /test/index.html 
title: Kategorie Bautagebuch
---


{% for post in site.categories.Bautagebuch %} 
<blockquote><div style="  display: grid; gap: 1em;  margin: 0em;">
<div style="width: 30px; height: 100%;"><h1 class="genericon genericon-{{ post.layout }}">&nbsp;</h1></div>
<div style="height: 100%;">
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
</div>
</div>
</blockquote>

{% endfor %}
