---
layout: default
title: The sitespeed.io blog
description: The team behind sitespeed.io
author: Peter Hedenskog
keywords: sitespeed.io, peter hedenskog, tobias lidskog
nav: blog
---

# Blog

{% for post in site.posts %}
  <img src="{{ post.authorimage }}" class="photo pull-left" width="100" height="100">

## [{{ post.title }}]({{ post.url }})

**{{ post.date | date: '%Y' }}{{ post.date | date: '%m' }}{{ post.date | date: '%d' }}** -
  {{ post.intro }}

  [>> Read more]({{ post.url }})

  * * *

{% endfor %}
