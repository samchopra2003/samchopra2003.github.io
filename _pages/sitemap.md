---
layout: portfolio-site
title: Sitemap
description: Pages and research papers on Samarth Chopra’s academic website.
permalink: /sitemap/
sitemap: false
noindex: true
---
<div class="wrap inner-page">
  <header class="page-intro"><h1>Sitemap</h1></header>
  <ul class="cv-list">
    <li><a href="{{ '/' | relative_url }}">Home</a></li>
    <li><a href="{{ '/publications/' | relative_url }}">Publications</a></li>
    <li><a href="{{ '/cv/' | relative_url }}">CV</a></li>
    {% assign publications = site.publications | sort: 'date' | reverse %}
    {% for publication in publications %}
    <li><a href="{{ publication.url | relative_url }}">{{ publication.title | escape }}</a></li>
    {% endfor %}
  </ul>
</div>
