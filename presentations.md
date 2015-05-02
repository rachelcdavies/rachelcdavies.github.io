---
layout: page
title: Presentations
permalink: /presentations/
---

I put my slides for past talks on [SlideShare](http://www.slideshare.net/RachelDavies) and here are links to some of them.

{% for video in site.videos %}
  [{{ video.title }}]({{ video.link }})
{% endfor %}