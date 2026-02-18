---
title: Home
---

Welcome.

---

## Recent posts

{% assign all_entries = site.posts | concat: site.notes | concat: site.psets %}
{% assign sorted_entries = all_entries | sort: "date" | reverse %}

{% for entry in sorted_entries limit:5 %}
- **[{{ entry.title }}]({{ entry.url }})**  
  <small>{{ entry.date | date: "%B %d, %Y" }}</small>

{% endfor %}
