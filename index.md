---
layout: default
title: Home
---

# Welcome to my blog 👋

I write about:

- Technology
- Learning notes
- Experiments and ideas

Stay curious 🚀

---

## 📚 Posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      - {{ post.date | date: "%Y-%m-%d" }}
    </li>
  {% endfor %}
</ul>
