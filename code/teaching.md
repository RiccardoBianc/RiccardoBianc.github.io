---
title: Teaching activities
layout: home
nav_order: 3
last_modified_date: July 17 2025 at 10:36 AM
---

# Teaching activities

{% for year in site.data.teaching %}
## Academic Year {{ year.year }}

{% for course in year.courses %}
- **{{ course.title }}**  
  {% if course.page %} · <a href="{{ course.page }}" target="_blank"> <i class="fa-solid fa-link"></i> Course website </a> {% endif %}
  {% endfor %}

---
{% endfor %}
