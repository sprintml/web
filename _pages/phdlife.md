---
title: "SprintML Lab - PhDLife"
layout: textlay
excerpt: "SpringML Lab -- PhDLife"
sitemap: false
permalink: /phdlife/
---

99 Pieces of PhD Advice
-----

Here, we share 99 advices on Ph.D. life based on our prior experience. We cover topics from starting a Ph.D. to reading and writing papers, and becoming a full member of the scientific community. If you have feedback or your own advise to share, please reach out!



{% for post in site.posts.phdlife reversed%}

### [{{ post.title | escape }}]({{ post.url | relative_url }})

Published: {{ post.date | date: "%b %-d, %Y" }} 
{% endfor %}