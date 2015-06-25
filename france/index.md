---
layout: page
title: France
excerpt: "Posts about France"
categories: france
search_omit: true
---

We're not in France yet, stay tuned.

<ul class="post-list">
{% for post in site.categories.france %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
