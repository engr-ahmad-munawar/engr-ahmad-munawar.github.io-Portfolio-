---
layout: default
title: Home
---

# 👋 Welcome to My Portfolio

Hi, I'm Ahmed — developer, learner, builder.

## 🚀 Explore
- Learn about me → [About](/about)
- My growth → [My Journey](/journey)
- Read my posts → [Blog](/blog)

---

## 🔥 Latest Posts
{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}
