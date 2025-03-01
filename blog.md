---
layout: page
title: Blog
permalink: /blog/
---

# Welcome to My Blog!

Here you can find my latest posts.

{% for post in site.posts %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.date | date_to_string }}</p>
  {{ post.excerpt }}
{% endfor %}
