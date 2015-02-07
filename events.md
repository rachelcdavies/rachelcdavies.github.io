---
layout: page
title: Events
permalink: /events/
---

I'll be presenting at these industry conferences and meetups.

{% for event in site.events %}
  {{ event.date | date: ' %d %B %Y '}} &raquo; [{{ event.title }}]({{ event.link }})
{% endfor %}
