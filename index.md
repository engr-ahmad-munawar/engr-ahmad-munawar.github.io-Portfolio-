---
title: Home
---

# 👋 Welcome to My Portfolio

Hi, I'm Ahmed — Developer & Learner 🚀  

## Navigation
- [About Me](/about)
- [My Journey](/journey)
- [Blog Posts](/blog)

---

## 📝 Latest Posts

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}
