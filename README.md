---
layout: home
title: "Home"
permalink: /
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{% link {{ post.relative_path }} %}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
