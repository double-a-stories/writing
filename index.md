---
layout: home
title: "Home"
permalink: /
---

{% for post in site.posts %}
- [{{ post.title }} {% for tag in post.tags %}<span class="tag">{{ tag | capitalize }}</span>]({{ post.url | relative_url }})  {% endfor%} {% if post.description %}-- {{ post.description }} {% endif %}
{% endfor %}
