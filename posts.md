---
layout: page
title: Posts
---

# Blog Posts 📝

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
No posts yet… stay tuned!
{% endif %}
