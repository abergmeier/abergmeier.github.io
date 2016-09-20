---
layout: blog
title: Blog
---

{% for post in site.categories.blog %}

<div>
  <h1 class="blog-post-title"><a href="{{ post.url }}">{{ post.title }}</a></h1>
  <div>
    <span>{{ post.date | date_to_long_string }}</span>
  </div>
  {{ post.content }}
</div>

{% endfor %}
