---
layout: page
title: Presentations
permalink: /presentations/
---

I uploaded my slides for past talks to [SlideShare](http://www.slideshare.net/RachelDavies)
Below you can find a list of videos of my keynotes, workshops and talks.

{% for video in site.videos %}
  [{{ video.title }}]({{ video.link }})
{% endfor %}