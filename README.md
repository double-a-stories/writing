---
layout: home
title: "Home"
permalink: /
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a> {% for tag in page.tags %}<span class="tag">{{ tag }}</span>{% endfor%} {% if post.description %}-- {{ post.description }} {% endif %}
    </li>
  {% endfor %}
</ul>
