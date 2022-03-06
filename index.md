---
layout: home
title: "Home"
permalink: /
---

{% for post in site.posts %}
- [{{ post.title }} {% for tag in post.tags %}<span class="tag">{{ tag | capitalize }}</span>  {% endfor%}]({{ post.url | relative_url }}) {% if post.description %}-- {{ post.description }} {% endif %}
{% endfor %}
