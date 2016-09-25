---
layout: blog
title: Blog about embedded
---

{% for post in site.categories.embedded_blog %}

<div>
  <h1><a href="{{ post.url }}">{{ post.title }}</a></h1>
  <div>
    <span>{{ post.date | date_to_long_string }}</span>
  </div>
  {{ post.content }}
</div>

{% endfor %}
