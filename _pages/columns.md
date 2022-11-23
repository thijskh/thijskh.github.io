---
layout: archive
permalink: /columns/
title: "Columns"
author_profile: true
taxonomy: categories
---

## Mijn laatste vijf columns

{% for post in site.posts limit:5 %}
### [{{post.title}}]({{post.url}}) ({%- include date-nl.html date=post.date -%})

{{post.excerpt}}

{% endfor %}

## Alle columns per categorie

{% for category in categories %}
* **[category.title]({{site.categories[category|first].url}})**
{% endfor %}
