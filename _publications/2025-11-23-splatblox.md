---
title: "Splatblox: Traversability-Aware Gaussian Splatting for Outdoor Robot Navigation"
short_title: Splatblox
collection: publications
category: manuscripts
permalink: /publication/2025-11-23-splatblox
date: 2025-11-23
venue: arXiv preprint
venue_short: arXiv preprint
authors:
  - Samarth Chopra
  - Jing Liang
  - Gershom Seneviratne
  - Yonghan Lee
  - Jaehoon Choi
  - Jianyu An
  - Stephen Cheng
  - Dinesh Manocha
excerpt: Combines RGB and LiDAR to map traversable terrain for robots navigating in dense vegetation.
paperurl: https://arxiv.org/abs/2511.18525
paper_label: arXiv
doi: 10.48550/arXiv.2511.18525
project_url: https://splatblox.github.io/
featured_order: 2
image: https://splatblox.github.io/static/images/overview_compressed-1.png
image_alt: Splatblox outdoor robot navigation system and traversability maps
---

Splatblox fuses camera segmentation and LiDAR point clouds into a traversability-aware Euclidean signed distance field. The robot updates the map as it moves so the planner can account for both obstacle geometry and terrain semantics. The paper reports field trials with a quadruped and demonstrates transfer to a wheeled robot.
