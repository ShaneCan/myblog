---
title: Recent Gains from reading research papers[Nov 10th]
author: Tianxiong Zhang
date: '2023-11-10'
slug: recent-gains-from-reading-research-papers-Nov-10th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2023-11-10T20:38:32+08:00'
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
#### [1] Yang S, Scherer S. CubeSLAM: Monocular 3D object detection and SLAM without prior models[J]. arXiv preprint arXiv:1806.00557, 2018.

This paper proposes a single-image 3D rectangular object detection and a multi-view object SLAM approach without a priori object modeling, and demonstrates that the two aspects can benefit from each other. For 3D detection, the paper generates high-quality rectangular proposals from 2D bounding boxes and vanishing point sampling. The proposals are further scored and selected to align with image edges. Experiments on SUN RGBD and KITTI demonstrate the efficiency and accuracy of existing methods. Then in the second part, multi-view beam adjustment with novel measurements is proposed to jointly optimize camera poses, objects and points using single view detection results. Objects can provide more geometric constraints and scale consistency than points.

**Note1:**
Most existing monocular approaches address object detection and SLAM separately and also rely on existing CAD models of objects that may not be applicable to general environments. The innovation of this work lies in focusing on a priori-free 3D object mapping and jointly addressing 3D object detection and multi-view object SLAM, proposing a system that addresses both 3D object detection and SLAM.

**Note2:**
This approach demonstrates for the first time that semantic object detection and geometric SLAM can be mutually beneficial in a unified framework, and the inclusion of 3D LIDAR can be considered in the future and integrated into a single framework.

