---
layout: page
permalink: /attendances/
title: Attendances
nav: true
nav_order: 5
---

This is a list of things I attended (or will attend if I update frequently).

{% assign attendances = site.data.attendances | sort: 'date' | reverse %}
{% for item in attendances %}
<details markdown="1"><summary>{{ item.title }} ({{ item.date | date: "%B %Y" }})</summary>

{{ item.description }}

</details>
{% endfor %}