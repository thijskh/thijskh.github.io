---
layout: archive
permalink: /columns/
title: "Columns"
author_profile: true
---

## Mijn laatste vijf columns

{% for post in site.posts limit:5 %}
<h3><a href="{{post.url}}">{{post.title}}</a> ({%- include date-nl.html date=post.date -%})</h3>

<p>
  {{ post.excerpt | strip_html }}
  <small><a href="{{ post.url | prepend: site.baseurl }}">(lees verder)</a></small>
</p>
{% endfor %}

## Alle columns per categorie

* **[De coronacrisis](/categories/#corona)**
* **[Het academisch bedrijf](/categories/#academisch-bedrijf)**
* **[Geboorte & dood](/categories/#geboorte-dood)**
* **[Van alles en nog wat](/categories/#alles-nogwat)**
