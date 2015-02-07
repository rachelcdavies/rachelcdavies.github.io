---
layout: page
title: Events
permalink: /events/
---

I'll be presenting at these upcoming industry conferences and meetups.

{% for event in site.events %}
  {{ event.date | date: ' %d %b %Y '}} &raquo; [{{ event.title }}]({{ event.link }})
{% endfor %}
