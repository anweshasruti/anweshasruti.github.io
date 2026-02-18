---
title: Notes
permalink: /notes/
---

{% for note in site.notes %}
- **[{{ note.title }}]({{ note.url }})**  
  <small>{{ note.date | date: "%B %d, %Y" }}</small>

{% endfor %}
