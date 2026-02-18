---
title: Home
---

Welcome.

---

## Recent Posts

{% for post in site.posts limit:5 %}
**[{{ post.title }}]({{ post.url }})**  
<small>{{ post.date | date: "%B %d, %Y" }}</small>

<br>
{% endfor %}
