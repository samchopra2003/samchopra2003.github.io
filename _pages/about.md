---
layout: portfolio-site
permalink: /
title: Samarth Chopra
seo_title: Samarth Chopra | Robotics PhD Student at Penn
description: Samarth Chopra is a robotics PhD student at the University of Pennsylvania's GRASP Lab and an NSF Graduate Research Fellow working on real-to-sim, robot navigation, and manipulation.
author_profile: false
sitemap: true
noindex: false
redirect_from:
  - /about/
  - /about.html
---
<section class="hero wrap" aria-labelledby="home-title">
  <div class="hero-copy">
    <p class="eyebrow">GRASP Lab · University of Pennsylvania</p>
    <h1 id="home-title">Samarth Chopra</h1>
    <p class="hero-lede">I build scene models for robots that navigate and manipulate in the physical world.</p>
    <p class="hero-bio">I’m a PhD student in Electrical and Systems Engineering at Penn’s <a href="https://www.grasp.upenn.edu/">GRASP Lab</a> and an NSF Graduate Research Fellow. My research uses 3D reconstruction and physical property estimation to build simulations for evaluating robot policies.</p>
    <div class="hero-actions">
      <a class="button" href="#research">Explore my research</a>
      <div class="hero-profiles">{% include profile-links.html %}</div>
    </div>
  </div>
  <figure class="portrait">
    <img src="{{ '/images/' | append: site.author.avatar | relative_url }}" alt="Samarth Chopra" width="600" height="720" fetchpriority="high">
  </figure>
</section>

<section id="research" class="research" aria-labelledby="research-title">
  <div class="wrap">
    <div class="section-heading">
      <h2 id="research-title">Selected research</h2>
      <a class="text-link" href="{{ '/publications/' | relative_url }}">All publications</a>
    </div>
    {% assign featured = site.publications | where_exp: 'publication', 'publication.featured_order != nil' | sort: 'featured_order' %}
    <div class="research-grid">
      {% for publication in featured %}
      <article class="research-card">
        <div class="card-image card-image--{{ publication.short_title | slugify }}">
          <img src="{{ publication.image | escape }}" alt="{{ publication.image_alt | escape }}" width="720" height="420" loading="lazy" decoding="async">
        </div>
        <div class="card-content">
          <p class="eyebrow">{{ publication.venue_short | escape }} · {{ publication.date | date: '%Y' }}</p>
          <h3><a href="{{ publication.url | relative_url }}">{{ publication.short_title | escape }}</a></h3>
          <p class="card-summary">{{ publication.excerpt | escape }}</p>
          {% include publication-links.html publication=publication %}
        </div>
      </article>
      {% endfor %}
    </div>
  </div>
</section>
