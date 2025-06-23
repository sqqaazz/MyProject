---
layout: default
title: Home
---

<!-- # 최신 글 -->

<div class="layout">

<section class="post-thumbnail">
  {% for post in site.posts %}
   <a href="{{ post.url }}" class="post-card-link">
    <div class="post-card">
      {% if post.image %}
        <div class="post-image-wrapper">
          <img src="{{ post.image }}" alt="{{ post.title }}" class="post-image">
        </div>
      {% endif %}
      <div class="post-content">
        <h3 class="post-title">
          <a href="{{ post.url }}">{{ post.title }}</a>
        </h3>
        <p class="post-excerpt">{{ post.excerpt }}</p>
      </div>
    </div>
   </a>
  {% endfor %}
  </section>

   {% include sidebar.html %}
</div>