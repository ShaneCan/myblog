---
title: Recent Gains from reading research papers[Mar 8th]
author: Tianxiong Zhang
date: '2024-03-08'
slug: recent-gains-from-reading-research-papers-Mar-8th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2024-03-08T20:38:32+08:00'
featured: no
draft: no
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/CpkOjOcXdUY)'
  focal_point: ""
  placement: 2
  preview_only: false
projects: []
summary: "Daily Paper Reading "
---
#### [1] Chen Y, Gu C, Jiang J, et al. Periodic vibration gaussian: Dynamic urban scene reconstruction and real-time rendering[J]. arXiv preprint arXiv:2311.18561, 2023.

This paper introduces a novel dynamic scene representation method called Periodic Vibration Gaussian (PVG), specifically designed for the reconstruction and real-time rendering of large-scale dynamic urban scenes. The PVG method effectively captures both static and dynamic elements in a scene by incorporating periodic vibration-based temporal dynamics. 

**Note1:**
 PVG is a unified representation model that introduces periodic vibration-based temporal dynamics, enabling each Gaussian point to have a specific lifespan and dynamically adjust its position and opacity based on temporal changes. This representation not only elegantly unifies static and dynamic scene elements but also captures the motion characteristics of dynamic objects, such as velocity and staticness, through periodic vibrations. By integrating periodic vibrations into the conventional 3D Gaussian splatting formulation, the PVG model provides a new approach to dynamic scene modeling.

**Note2:**
To enhance temporal coherence in representation learning with typically sparse training data, the article proposes a scene flow-based temporal smoothing mechanism that estimates the state changes between adjacent timestamps to smooth the scene flow. Additionally, to more effectively represent unbounded urban scenes, the article introduces a position-aware adaptive control strategy that adaptively adjusts the size of the point cloud based on its location, thereby reducing the number of required points while maintaining scene accuracy.