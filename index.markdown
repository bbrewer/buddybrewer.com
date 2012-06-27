---
layout: default
title: Buddy Brewer
description: Web performance entrepreneur, CrossFitter, NASCAR fan. I like things that go fast.
---

# Blog Posts

{% for post in site.posts limit:5 %}

**<a href="{{ post.url }}">{{ post.title }}</a>**<br>
*Posted on {{ post.date | date_to_long_string }}*

{% endfor %}

---------------------------------------------------------------

# Talks and Contributed Articles

[**A Practical Guide to the Navigation Timing API**](http://calendar.perfplanet.com/2011/a-practical-guide-to-the-navigation-timing-api/) - December 16, 2011<br>
*2011 Performance Calendar, Planet Performance*

[**High Speed Web Sites At Scale**](http://www.slideshare.net/buddybrewer/high-speed-web-sites-at-scale) - October 3, 2011<br>
*HighLoad++ (Moscow, Russia)*
