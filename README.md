---
layout: home
title: "Home"
permalink: /
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{% post_url {{post.name}} %}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
