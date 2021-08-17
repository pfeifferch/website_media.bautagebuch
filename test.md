---
layout: default
permalink: /test/index.html 
title: Kategorie Bautagebuch
---

<style>
    generiquote { 
       background-color: grey;
       color: white;
       text-align: center; 
       margin-left: 40px /*.4em*/
       margin-top: 100px
       position: relative;
    }
generiquote:before {
   content: "\f471";
   background-color: #bfb;
   top: -100px;
   height: 100px;
   width: 100%;
   position: absolute;
}
</style>
&\f471;
{% for post in site.categories.Bautagebuch %} 

<div class="generiquote genericon genericon-{{ post.layout }}">
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

{% endfor %}
