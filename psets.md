---
title: Psets
permalink: /psets/
---

{% for pset in site.psets %}
- **[{{ pset.title }}]({{ pset.url }})**  
  <small>{{ pset.date | date: "%B %d, %Y" }}</small>

{% endfor %}
