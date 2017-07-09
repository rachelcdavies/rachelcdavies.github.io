---
layout: page
title: Talks
permalink: /talks/
---

I put my slides for past talks on [SlideShare](http://www.slideshare.net/RachelDavies) and below are links to some videos.

{% for video in site.videos reversed %}
  [{{ video.title }}]({{ video.link }})
{% endfor %}




