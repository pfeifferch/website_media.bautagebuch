---
layout: default
permalink: /test/index.html 
title: Kategorie Bautagebuch
---
<style>
#kuller {
 margin: auto;
 width: 45px;
 height: 45px;
 background-color: #000;
 color: #637d96;
 border-radius: 360px;
 text-align: center;
 vertical-align: middle;
 font-size: 35px;
 margin-top: 5px;
 padding-left: -150px;
 }
</style>


{% for post in site.categories.Bautagebuch %} 
<blockquote>
<div style="width: 30px; height: 100%;"><h1 id="kuller" class="genericon genericon-{{ post.layout }}">&nbsp;</h1></div>
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
</blockquote>

{% endfor %}
