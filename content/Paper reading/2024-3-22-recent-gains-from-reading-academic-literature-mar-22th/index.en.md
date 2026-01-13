---
title: Recent Gains from reading research papers[Mar 22th]
author: Tianxiong Zhang
date: '2024-03-22'
slug: recent-gains-from-reading-research-papers-Mar-22th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2024-03-22T20:38:32+08:00'
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
#### [1] Zhou X, Lin Z, Shan X, et al. Drivinggaussian: Composite gaussian splatting for surrounding dynamic autonomous driving scenes[J]. arXiv preprint arXiv:2312.07920, 2023.

The literature introduces DrivingGaussian, specifically designed for efficiently representing and modeling dynamic autonomous driving scenarios. By employing Composite Gaussian Splatting technology, it decomposes the static background and multiple dynamic objects separately and reconstructs them for global rendering in complex driving scenarios. The framework utilizes incremental static 3D Gaussians to gradually build the static background of the entire scene and employs composite dynamic Gaussian maps to handle multiple moving objects, thereby restoring their accurate positions and occlusion relationships in the scene. Furthermore, DrivingGaussian leverages LiDAR data as prior knowledge to achieve more detailed scene reconstruction and maintain panoramic consistency. This method surpasses existing technologies in dynamic driving scene reconstruction and can achieve high fidelity and multi-camera consistent panoramic view synthesis.

**Note 1:**
Composite Gaussian Splatting is a core concept of DrivingGaussian. It decomposes the entire scene into a static background and dynamic objects, then reconstructs each part separately, and finally integrates them for global rendering. Specifically, the paper first uses incremental static 3D Gaussians to build a comprehensive scene sequentially obtained from multiple surrounding camera views. Then, it uses composite dynamic Gaussian maps to individually reconstruct each moving object and dynamically integrates them into the static background based on the Gaussian maps. This method allows for efficient representation and rendering of dynamic objects and static backgrounds in complex driving scenarios.

**Note 2:** 
DrivingGaussian uses LiDAR data as prior knowledge for Gaussian Splatting to recover more accurate geometric structures and maintain multi-view consistency. Compared with traditional Structure from Motion (SfM) based initialization methods, LiDAR prior provides more accurate geometric shape priors and comprehensive scene descriptions, not just as depth supervision for images. This method enables DrivingGaussian to demonstrate the potential to reconstruct large-scale dynamic scenes even without LiDAR data, and provide more accurate geometric structures and better multi-view consistency when LiDAR data is available.

**Note 3:** 
The paper mentions that the model faces certain challenges when dealing with extremely small objects (such as roadside stones) and materials with full reflection characteristics (such as glass mirrors and water surfaces). Future work can focus on improving Gaussian Splatting technology to better represent these areas with complex lighting and reflection characteristics.