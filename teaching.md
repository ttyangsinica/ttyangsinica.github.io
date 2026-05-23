---
layout: page
title: "Teaching"
permalink: /teaching/
---

{% for term in site.data.courses %}
## {{ term.term }}{% if term.institution %} ({{ term.institution }}){% endif %}

{% for course in term.courses %}
- {% if course.url %}[{{ course.title }}]({{ course.url }}){% else %}{{ course.title }}{% endif %}{% if course.title_zh %} ({{ course.title_zh }}){% endif %}
{% endfor %}
{% endfor %}
