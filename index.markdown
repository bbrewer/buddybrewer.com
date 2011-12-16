---
layout: default
title: Buddy Brewer
description: Web performance consultant and co-founder of Log Normal.
---

# Blog Posts

{% for post in site.posts limit:5 %}

**<a href="{{ post.url }}">{{ post.title }}</a>**<br>
*Posted on {{ post.date | date_to_long_string }}*

{% endfor %}

---------------------------------------------------------------

# Talks and Contributed Articles

[**High Speed Web Sites At Scale**](http://www.slideshare.net/buddybrewer/high-speed-web-sites-at-scale) - October 3, 2011<br>
*HighLoad++ (Moscow, Russia)*
