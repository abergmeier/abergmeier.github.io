---
layout: blog
title: Blog about embedded
---

<header>My blog about all things hardware and low-level programming. Documents my tinkering phases.</header>

{% for post in site.categories.embedded_blog %}

<div>
  <h1><a href="{{ post.url }}">{{ post.title }}</a></h1>
  <div>
    <span>{{ post.date | date_to_long_string }}</span>
  </div>
  {{ post.content }}
</div>

{% endfor %}
