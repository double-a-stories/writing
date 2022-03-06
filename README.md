---
layout: home
title: "Home"
permalink: /
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ site.url | append: post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
