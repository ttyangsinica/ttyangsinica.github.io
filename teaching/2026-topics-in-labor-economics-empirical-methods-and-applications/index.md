---
layout: page
title: "Topics in Labor Economics (2026 Spring)"
permalink: /teaching/2026-topics-in-labor-economics-empirical-methods-and-applications/
---

{% assign course = site.data.labor_economics_2026 %}

<div class="course-meta">
  <div>
    <span class="meta-label">Course</span>
    <strong>{{ course.title }}</strong><br>
    <span>{{ course.title_zh }}</span>
  </div>
  <div>
    <span class="meta-label">Term</span>
    <strong>{{ course.term }}</strong><br>
    <span>{{ course.institution }}</span>
  </div>
</div>

{% if course.syllabus_url %}
[Syllabus]({{ course.syllabus_url }})
{% endif %}

## Suggestive Textbooks

{% for book in course.textbooks %}
- {% if book.url %}[{{ book.authors }}{% if book.year %} ({{ book.year }}){% endif %}, {{ book.title }}]({{ book.url }}){% else %}{{ book.authors }}{% if book.year %} ({{ book.year }}){% endif %}, {{ book.title }}{% endif %}
{% endfor %}

## Learning Resources

{% for resource in course.resources %}
- {% if resource.url %}[{{ resource.title }}]({{ resource.url }}){% else %}{{ resource.title }}{% endif %}
{% endfor %}

## Class Data

{% for item in course.class_data %}
- {% if item.url %}[{{ item.title }}]({{ item.url }}){% else %}{{ item.title }}{% endif %}
{% endfor %}

## Class Slides

<div class="schedule-list">
{% for week in course.schedule %}
  <section class="schedule-week">
    <h3>{{ week.date }}</h3>
    <ul>
      {% for item in week.items %}
        <li>{% if item.url %}<a href="{{ item.url }}">{{ item.title }}</a>{% else %}{{ item.title }}{% endif %}</li>
      {% endfor %}
    </ul>
  </section>
{% endfor %}
</div>
