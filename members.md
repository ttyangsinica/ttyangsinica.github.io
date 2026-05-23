---
layout: page
title: "Members"
permalink: /members/
---

{% for group in site.data.members %}
## {{ group.category }}

{% for person in group.people %}
- {{ person.name }}{% if person.affiliation %} ({{ person.affiliation }}){% endif %}
{% endfor %}
{% endfor %}
