---
title: "SprintML Lab - Blog"
layout: textlay
excerpt: "SpringML Lab -- Blog"
sitemap: false
permalink: /blog/
---

Posts
-----

{% for post in site.posts reversed%}

### [{{ post.title | escape }}]({{ post.url | relative_url }})

Published: {{ post.date | date: "%b %-d, %Y" }} {% endfor %}

### [How to Keep a Model Stealing Adversary Busy?](http://www.cleverhans.io/2022/04/21/pow-defense.html)

Published: Apr 21, 2022

### [All You Need Is Matplotlib](http://www.cleverhans.io/2022/04/17/fl-privacy.html)

Published: Apr 17, 2022

### [Beyond federation: collaborating in ML with confidentiality and privacy](http://www.cleverhans.io/2021/05/01/capc.html)

Published: May 1, 2021
