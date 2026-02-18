---
title: Home
---

Hello! My name is Anwesha Paul, and I am currently a high school student. I have a lot of pretty varied interests, but some things I love especially are linguistics, mathematics, computer science, geography, and sociology. I think this site is mainly going to focus on linguistics for now, along with my very random rants on topics I think are interesting haha. Maybe I'll share some notes here, or post solutions to psets:) Also, this is pretty random, but [here](https://letterboxd.com/anweshasruti/list/filmlist:80704112/) are some films I particularly love!

My email is `anwesha at tuta.io` and my username is `anweshasruti` on pretty much everything I use.

---

## Recent posts

{% assign all_entries = site.posts | concat: site.notes | concat: site.psets %}
{% assign sorted_entries = all_entries | sort: "date" | reverse %}

{% for entry in sorted_entries limit:5 %}
- **[{{ entry.title }}]({{ entry.url }})**  
  <small>{{ entry.date | date: "%B %d, %Y" }}</small>

{% endfor %}
