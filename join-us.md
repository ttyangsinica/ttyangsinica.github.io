---
layout: page
title: "Join Our Research Group"
permalink: /join-us/
---

{% for item in site.data.openings %}
- {% if item.url %}[{{ item.title }}]({{ item.url }}){% else %}{{ item.title }}{% endif %}{% if item.note %} {{ item.note }}{% endif %}
{% endfor %}
