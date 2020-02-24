---
layout: page
title: Cats
---

# Cats

If my blog were a collection of cats insted of posts, I'd have {{ site.posts.size }} cats

## Right Now I have 6 Cats
{% for cat in site.data.cats %}
* {{ cat.name }}
{% endfor %}

Tigger is our oldest cat.
{% for cat in site.data.cats %}
{% if cat.name == 'Tigger' %}
  He is {{ cat.age }} years old.
{% endif %}
{% endfor %}
Unfortunately, he has a tumor in his mouth.
![picture of Tigger](../img/Tigger.jpg){: #Tigger}