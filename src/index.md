---
title: Luz Dice
layout: "main.njk"
---
Bienvenidos locos

{% for post in collections.posts %}
- **{{ post.data.title }}** ({{ post.data.date | date: "%d/%m/%Y" }})  
  [Leer más]({{ post.url }})
{% endfor %}

