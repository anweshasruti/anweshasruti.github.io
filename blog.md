---
title: Blog
permalink: /blog/
---

{% for post in site.posts %}
<div style="margin-bottom: 28px;">
  <div style="font-size: 1.25em;">
    <a href="{{ post.url }}">{{ post.title }}</a>
  </div>
  <div style="font-size: 0.9em; color: #666;">
    {{ post.date | date: "%B %d, %Y" }}
  </div>
</div>
{% endfor %}
