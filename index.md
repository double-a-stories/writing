---
layout: home
title: "Home"
permalink: /
---

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) {% for tag in page.tags %}<span class="tag">{{ tag }}</span> {% endfor%} {% if post.description %}-- {{ post.description }} {% endif %}
{% endfor %}
