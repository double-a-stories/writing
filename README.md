---
layout: home
title: "Home"
permalink: /
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>  {{ post.relative_path }} 
    </li>
  {% endfor %}
</ul>
