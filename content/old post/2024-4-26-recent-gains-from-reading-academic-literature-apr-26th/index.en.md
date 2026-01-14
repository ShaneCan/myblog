---
title: Recent Gains from reading research papers[Apr 26th]
author: Tianxiong Zhang
date: '2024-04-26'
slug: recent-gains-from-reading-research-papers-Apr-26th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2024-04-26T20:38:32+08:00'
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
#### [1]Yan C, Qu D, Wang D, et al. Gs-slam: Dense visual slam with 3d gaussian splatting[J]. arXiv preprint arXiv:2311.11700, 2023.

The paper presents a novel dense visual SLAM system, GS-SLAM, which for the first time utilizes a 3D Gaussian representation method in a SLAM system. GS-SLAM achieves a better balance between efficiency and accuracy, and compared to recent SLAM methods using neural implicit representations, it adopts a real-time differentiable splatting rendering pipeline, significantly accelerating map optimization and RGB-D rendering.

**Note 1:**
One of the core innovations of the paper is the adaptive 3D Gaussian expansion strategy. This strategy effectively reconstructs newly observed scene geometry by adding new or removing noisy 3D Gaussians and improves the mapping of previously observed areas, which is crucial for expanding the 3D Gaussian representation to reconstruct the entire scene rather than synthesizing static objects in existing methods.

**Note 2:**
Another innovation of the paper is the introduction of a coarse-to-fine tracking technique. During the pose tracking process, an efficient coarse-to-fine technique is designed for selecting reliable 3D Gaussian representations to optimize the camera pose, thereby reducing runtime and enhancing the robustness of the estimation.

**Note 3:**
The method in the paper may be limited under certain conditions if the quality of the depth data is not high. Moreover, although the 3D Gaussian representation performs well in rendering and mapping, in some cases, such as in more challenging scenes in the TUM-RGBD dataset, further optimization may be required to improve tracking accuracy.