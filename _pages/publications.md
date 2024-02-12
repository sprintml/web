---
title: "SprintML Lab - Publications"
layout: textlay
#excerpt: "SprintML Lab -- Publications."
sitemap: false
permalink: /publications/
---

{% for y in site.years %}

### {{y}}

{% bibliography -f publications.bib -q @*[year={{y}}]* %}
{% endfor %}
