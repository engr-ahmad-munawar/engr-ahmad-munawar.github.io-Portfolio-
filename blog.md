---
layout: default
title: Blog
---

# 📝 My Blog

## 📢 Create a Post

👉 To add a post:
- Go to `_posts` folder
- Create file like:
  `YYYY-MM-DD-title.md`

---

## 📚 All Posts

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url }})
- {{ post.date | date: "%B %d, %Y" }}

{% endfor %}
