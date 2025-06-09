---
title: Teaching activities
layout: home
nav_order: 3
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
