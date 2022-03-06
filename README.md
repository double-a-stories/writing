---
layout: home
title: "Home"
permalink: /
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{% post_url {{ post.relative_path }} %}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
