---
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
---
layout: default
title: "Second Blog"
permalink: /second-blog/
date: 2026-04-03
---

<!-- You can add content here later -->
{% endfor %}
