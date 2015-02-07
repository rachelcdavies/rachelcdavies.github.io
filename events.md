---
layout: page
title: Events
permalink: /events/
---

{% for event in site.events %}
  {{ event.date | date: ' %d %B %Y '}} &raquo; [{{ event.title }}]({{ event.link }})
{% endfor %}
