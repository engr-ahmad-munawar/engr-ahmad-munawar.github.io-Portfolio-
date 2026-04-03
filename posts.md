---
layout: page
title: Posts
---

<div class="hero" style="background:#2575fc; color:#fff; padding:2rem; border-radius:15px; text-align:center;">
  <h1>Blog Posts 📝</h1>
  <p>Projects, tutorials, and tech musings</p>
</div>

{% if site.posts.size > 0 %}
<div class="posts-grid">
{% for post in site.posts %}
<div class="post-card">
- [**{{ post.title }}**]({{ post.url }})  
  _{{ post.date | date: "%b %-d, %Y" }}_  
  {{ post.excerpt | truncatewords: 25 }}
</div>
{% endfor %}
</div>
{% else %}
<p>No posts yet… stay tuned!</p>
{% endif %}
