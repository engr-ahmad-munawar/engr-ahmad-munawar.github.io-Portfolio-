---
title: Blog
---

# My Blog

## 📝 Create New Post
> Click here to create a new post:  
> [➕ Add Post](https://github.com/engr-ahmad-munawar/engr-ahmad-munawar.github.io/new/main/_posts)  

> **Tip:** Name file like `YYYY-MM-DD-title.md`  
> Add front matter:  
> ```
> ---
> layout: post
> title: "Post Title"
> date: 2026-04-03
> ---
> ```
> Write content in Markdown below.

---

## All Posts

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url }})
- {{ post.date | date: "%B %d, %Y" }}
{% endfor %}
