---
layout: page
permalink: /publications/
title: Publications
description: 
nav: true
nav_order: 3
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{%- if site.enable_publication_search %}
  {% include bib_search.liquid %}
{%- endif %}

<div class="publications">

{% bibliography %}

</div>

