---
layout: page
title: Scotland
excerpt: "Posts about Scotland"
search_omit: true
---

Visit us later for some Scotland content!

<ul class="post-list">
{% for post in site.categories.scotland %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
