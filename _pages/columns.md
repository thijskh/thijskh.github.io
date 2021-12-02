---
layout: archive
permalink: /columns/
title: "Columns"
author_profile: true
---

{% for post in site.posts %}

* _{{ post.date | date: '%Y-%m-%d' }}_: {{ post.excerpt }}

{% endfor %}

