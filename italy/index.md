---
layout: page
title: Italy
excerpt: "Posts about Italy"
search_omit: true
categories: italy
---

<ul class="post-list">
{% for post in site.categories.italy %} 
{% if post.author %}
    {% assign author = site.data.authors[post.author] %}{% else %}{% assign author = site.owner %}
{% endif %}
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} {% if post.author %}<i><font size="2">by {{author.name}}</font></i>{% endif %} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
