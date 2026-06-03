---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* Ph.D. in Electrical and Systems Engineering, University of Pennsylvania
* B.S. in Electrical and Computer Engineering, University of Pittsburgh

Research
======
* Graduate Researcher, GRASP Lab
* Research areas: robotics, computer vision, embodied AI, Gaussian Splatting, simulation, and vision-language-action models

Honors
======
* NSF Graduate Research Fellowship Program

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
