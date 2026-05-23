---
layout: page
title: "Research"
permalink: /research/
---

## Working Papers

{% for paper in site.data.working_papers %}
- {% if paper.url %}[{{ paper.title }}]({{ paper.url }}){% else %}{{ paper.title }}{% endif %}{% if paper.authors %} ({{ paper.authors }}){% endif %}{% if paper.status %}, {{ paper.status }}{% endif %}
{% endfor %}

## Publications

{% for paper in site.data.publications %}
- {% if paper.url %}[{{ paper.title }}]({{ paper.url }}){% else %}{{ paper.title }}{% endif %}{% if paper.authors %} ({{ paper.authors }}){% endif %}{% if paper.journal %}, {{ paper.journal }}{% endif %}{% if paper.year %}, {{ paper.year }}{% endif %}
{% endfor %}
