---
layout: default
title: Blog
------
layout: default
title: Blog
permalink: /blog/
---

# 🔥 My Blog

<a href="{{ site.baseurl }}/create-post/" class="create-btn">
  + Create Post
</a>

---

{% for post in site.posts %}

## [{{ post.title }}]({{ site.baseurl }}{{ post.url }})

📅 {{ post.date | date: "%B %d, %Y" }}

---

{% endfor %}

# Blog Posts

[Create New Post](/blog/new-post)  
*(For GitHub Pages, posts are `.md` in `_posts/` folder)*
