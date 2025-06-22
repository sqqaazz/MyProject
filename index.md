---
layout: default
title: Home
---

<!-- # 최신 글 -->

<div class="post-thumbnails">
  {% for post in site.posts %}
    <div class="post-card">
      {% if post.image %}
        <img src="{{ post.image }}" alt="{{ post.title }}" class="post-image">
      {% endif %}
      <h3 class="post-title">
        <a href="{{ post.url }}">{{ post.title }}</a>
      </h3>
      <p class="post-excerpt">{{ post.excerpt }}</p>
      <a href="{{ post.url }}" class="read-more">Read more →</a>
    </div>
  {% endfor %}
</div>