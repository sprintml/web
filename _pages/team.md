---
title: "SprintML Lab - Team"
layout: gridlay
excerpt: "SprintML Lab: Team"
sitemap: false
permalink: /team/
---


Principal Investigators
=======================

{% assign pis = site.members | where: 'position', 'Principal Investigator' %} 

{% for pi in pis %}
[![](/assets/images/members/{{ pi.short_name }}.jpg)
{{ pi.name }}
=============
### Professor
#### {{pi.email}}
]({{pi.url}})

{% endfor %}

Lab Members
===========

{% assign count = 0 %} {% assign current\_members = site.members | where: 'active', true %} {% for person in current\_members %} {% assign count = count | plus: 1 %} {% if forloop.first %}

{% else %} {% endif %}

[

![](/assets/images/members/{{ person.short_name }}.jpg)

{{ person.name }}
-----------------

### {{person.position}}

#### {{ person.email}}





]({{person.url}})

{% if count >= 3 and forloop.last == false %}

{% assign count = 0 %} {% elsif forloop.last %}

{% endif %} {% endfor %}
