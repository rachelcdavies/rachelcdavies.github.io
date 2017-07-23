---
layout: post
title:  "Moving from Typepad to Jekyll"
date:   2015-01-05 16:18:09
---

I recently migrated this website from Typepad to [Github pages](https://pages.github.com/) using [Jekyll](http://jekyllrb.com/). Here are some of the reasons why and some tips on getting started with Jekyll.

My main reason for moving away from Typepad is to simplify the layout of my blog. I'm no longer in the consulting game and also wish to retire my ancient website -- thrown together in PHP one rainy Sunday more than 10 years ago! Nowadays, I'd like a simple website around my blog with as little hassle required polishing posts. When both these moves are complete, I'll also save a few pennies on hosting costs.

My usual pattern is to write my blog posts as plain text files while I'm offline on the train to London. I was used to pushing these into Typepad when I  eventually got online. One of the fiddly bits in moving from a plain text draft was positioning photos with related text using Typepad platform. I was attracted to Jekyll as it enables me to edit pages on my laptop using a basic text editor and check what they look like by running locally before pushing them to [GitHub](https://github.com/rachelcdavies).

I already had a GitHub account so getting started with [Github pages](https://pages.github.com/) was straightforward. Next I downloaded [Jekyll](http://jekyllrb.com/) which has plenty of helpful documentation. I exported my posts from Typepad and ran [typepad_to_jekyll](https://github.com/dams/typepad_to_jekyll). Now running locally, I could see that everything I'd written since 2004 was safely over!

I did a bit of tinkering with layout after reading some tips from [Joshua Lande](http://joshualande.com/jekyll-github-pages-poole/). I decided not to enable comments as I'd like to move discussion over to [Twitter](https://twitter.com/rachelcdavies) so I've implemented his Twitter plug on my blog posts.

I also wanted an [Events](http://rachelcdavies.github.io/events/) page generated from simple markdown files listing name and link of event and was very happy how quick this was to put together. See snippet below.

{% highlight html %}
{% raw %}
{% for event in site.events %}
  {{ event.date | date: ' %d %b %Y '}} &raquo; [{{ event.title }}]({{ event.link }})
{% endfor %}
{% endraw %}
{% endhighlight %}

My new site is still work-in-progress, many photos embedded in old posts link to images on Typepad -- I'll be gradually trawling through to clean those up. The site also has rather a vanilla look to it for now. But I'm happy with my new site and definitely have a smoother workflow for new posts. Please alert me to any glitches you spot with it.
