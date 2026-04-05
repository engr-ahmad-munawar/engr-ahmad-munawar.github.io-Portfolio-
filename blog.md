
---
layout: default
title: Blog
---

<div class="blog-header">
  <h1>Recent Posts ✍️</h1>
  <p>Exploring systems, code, and engineering concepts.</p>
</div>

<ul class="post-list">
  {% for post in site.posts %}
    <li class="post-item">
      <span class="post-date">{{ post.date | date: "%b %d, %Y" }}</span>
      <a class="post-link" href="{{ post.url | relative_url }}">
        {{ post.title }}
      </a>
    </li>
  {% else %}
    <li class="no-posts">
      <p>Stay tuned! I'll be sharing my first technical post soon.</p>
    </li>
  {% endfor %}
</ul>

<style>
  .blog-header {
    text-align: center;
    margin-bottom: 3rem;
  }

  .post-list {
    list-style: none;
    padding: 0;
  }

  .post-item {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 0;
    border-bottom: 1px solid rgba(255, 255, 255, 0.1);
  }

  .post-date {
    font-size: 0.9rem;
    color: #888;
    min-width: 120px;
  }

  .post-link {
    font-size: 1.2rem;
    color: #00bfff;
    text-decoration: none;
    font-weight: 500;
    flex-grow: 1;
    text-align: right;
  }

  .post-link:hover {
    color: #ff3860;
    text-decoration: underline;
  }

  .no-posts {
    text-align: center;
    padding: 2rem;
    color: #888;
    background: rgba(255, 255, 255, 0.05);
    border-radius: 8px;
  }
</style>

