---
layout: default
title: Home
---

<h1>🚀 Welcome to my blog</h1>

<p>I write about technology, learning notes, experiments and ideas.</p>

<hr>

<div class="posts-grid">
  {% for post in site.posts %}
  <div class="post-card">
    
    <h2 class="post-title">
      <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    </h2>

    <p class="post-date">
      📅 {{ post.date | date: "%Y-%m-%d" }}
    </p>

    <p class="post-excerpt">
      {{ post.excerpt | strip_html | truncate: 120 }}
    </p>

    <a class="read-more" href="{{ site.baseurl }}{{ post.url }}">
      Read More →
    </a>

  </div>
  {% endfor %}
</div>
