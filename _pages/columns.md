---
layout: archive
permalink: /columns/
title: "Columns"
author_profile: true
---

Een tamelijk volledige selectie van mijn columns – zie ook [de website van _Trouw_](https://www.trouw.nl/auteur/hieke-huistra).


{% for category in site.categories %}
{% capture category_name %}{{ category | first }}{% endcapture %}
## {{ category_name }}

{% for post in site.categories[category_name] %}
{{ post.date| date_to_long_string  }}: [{{post.title}}]({{post.url}})

{% endfor %}

{% endfor %}
