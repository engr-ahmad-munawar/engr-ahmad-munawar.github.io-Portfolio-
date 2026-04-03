---
layout: default
title: Blog
---

<h1>My Blog 📝</h1>
<p>Click the button below to create a new post directly on GitHub:</p>

<a href="https://github.com/engr-ahmad-munawar/engr-ahmad-munawar.github.io/new/main/_posts" target="_blank">
  <button>New Post ➕</button>
</a>

<hr>

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
