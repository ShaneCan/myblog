---
title: Recent Gains from reading research papers[Apr 5th]
author: Tianxiong Zhang
date: '2024-04-05'
slug: recent-gains-from-reading-research-papers-Apr-5th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2024-04-05T20:38:32+08:00'
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
#### [1] C. Jiang et al., "H 2 -Mapping: Real-Time Dense Mapping Using Hierarchical Hybrid Representation," in IEEE Robotics and Automation Letters, vol. 8, no. 10, pp. 6787-6794, Oct. 2023, doi: 10.1109/LRA.2023.3313051.

This paper introduces a novel real-time dense mapping method named H2-Mapping, which is based on Neural Radiance Field (NeRF) technology. The innovation lies in its ability to achieve high-quality 3D map reconstruction and real-time capabilities on edge computing devices. The method proposes a novel hierarchical hybrid representation that utilizes implicit multi-resolution hash encoding and explicit octree-based Signed Distance Function (SDF) priors to describe scenes at varying levels of detail. This representation allows for rapid initialization of scene geometry and facilitates easier learning of scene geometry. Additionally, the paper presents a coverage-maximizing keyframe selection strategy to address the forgetting issue and enhance mapping quality, especially in edge regions.

**Note 1:**
The hierarchical hybrid representation employed in this paper combines explicit octree SDF priors and implicit multi-resolution hash encoding to describe different levels of scene detail. By efficiently capturing coarse geometric shapes using octree SDF priors, the multi-resolution hash encoding can focus on residual geometric shapes, which are simpler than the complete geometry, thus improving geometric precision and convergence rates. This representation also achieves real-time dense mapping and dynamic scalability through rapid scene geometry initialization and geometry shapes that are easier to learn.

**Note 2:**
To achieve higher mapping accuracy, the paper proposes a coverage-maximizing keyframe selection strategy to address the critical forgetting issue in online mapping tasks. This strategy avoids redundant computation of samples across all keyframes, ensuring the quality of edge regions without increasing the number of training samples. Through this strategy, all allocated voxels are covered, improving the mapping quality with the least number of iterations, especially in edge areas.

**Note 3:** 
Current methods may face challenges when dealing with dynamic scenes, as dynamic objects can move or change during the mapping process. Future research could explore how to effectively integrate real-time data of dynamic objects to achieve accurate mapping of dynamic environments.
