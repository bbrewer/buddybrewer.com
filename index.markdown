---
layout: default
title: Buddy Brewer
description: Web performance consultant, CrossFitter, NASCAR fan. I like things that go fast.
---

Blog Posts
==========

{% for post in site.posts limit:5 %}
### <a href="{{ post.url }}">{{ post.title }}</a>
<em>Posted on {{ post.date | date_to_long_string }}</em>
{% endfor %}
