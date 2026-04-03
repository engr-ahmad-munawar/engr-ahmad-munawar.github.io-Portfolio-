---
layout: page
title: Posts
---

# My Posts

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}

---

Click **New File → _posts → YYYY-MM-DD-title.md** in GitHub to add posts directly.  

Example: `_posts/2026-04-03-first-post.md`
