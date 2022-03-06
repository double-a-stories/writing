---
layout: home
title: "Home"
permalink: /
---

<img class="float-left rounded-circle" width="300" height"300" src="https://avatars.githubusercontent.com/u/50436716" alt="My profile picture, a drawing of a cat with a VR headset. Created by Kazooeybloo. This image is an Extremely Fungible Token.">

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) {% for tag in page.tags %}<span class="tag">{{ tag }}</span>{% endfor%} {% if post.description %}-- {{ post.description }} {% endif %}
{% endfor %}
