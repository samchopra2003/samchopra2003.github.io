---
layout: portfolio-site
title: CV
description: Samarth Chopra’s education, research experience, honors, and publications in robotics.
permalink: /cv/
author_profile: false
sitemap: true
noindex: false
redirect_from:
  - /resume
---
<div class="wrap inner-page">
  <header class="page-intro">
    <h1>Curriculum vitae</h1>
    <p>Samarth Chopra · Robotics PhD student at the University of Pennsylvania</p>
  </header>
  <div class="cv-content">
    <section aria-labelledby="education-title">
      <h2 id="education-title">Education</h2>
      <ul class="cv-list">
        <li><strong>University of Pennsylvania</strong><span>PhD in Electrical and Systems Engineering, in progress</span></li>
        <li><strong>University of Pittsburgh</strong><span>BS in Electrical and Computer Engineering, 2025</span></li>
      </ul>
    </section>
    <section aria-labelledby="research-cv-title">
      <h2 id="research-cv-title">Research</h2>
      <ul class="cv-list">
        <li><strong>GRASP Lab, University of Pennsylvania</strong><span>Graduate researcher working on real-to-sim for manipulation and navigation</span></li>
      </ul>
    </section>
    <section aria-labelledby="honors-title">
      <h2 id="honors-title">Honors</h2>
      <ul class="cv-list">
        <li><strong>NSF Graduate Research Fellowship</strong><span>2025</span></li>
      </ul>
    </section>
    <section aria-labelledby="publications-cv-title">
      <h2 id="publications-cv-title">Publications</h2>
      <ul class="cv-list">
        {% assign publications = site.publications | sort: 'date' | reverse %}
        {% for publication in publications %}
        <li>
          <a href="{{ publication.url | relative_url }}">{{ publication.title | escape }}</a>
          <span>{{ publication.venue_short | escape }} · {{ publication.date | date: '%Y' }}</span>
        </li>
        {% endfor %}
      </ul>
    </section>
  </div>
</div>
