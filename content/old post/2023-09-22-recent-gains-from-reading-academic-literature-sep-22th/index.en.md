---
title: Recent Gains from reading research papers[Sep 22th]
author: Tianxiong Zhang
date: '2023-09-22'
slug: recent-gains-from-reading-research-papers-Sep-22th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2023-09-22T20:38:32+08:00'
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
#### [1]Duffhauss F, Baur S A. PillarFlowNet: A real-time deep multitask network for LiDAR-based 3D object detection and scene flow estimation[C]//2020 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS). IEEE, 2020: 10734-10741.

This paper focuses on realizing the combination of scene stream detection and target detection for 3D point clouds. Previously, scene flow estimation and target detection need to be processed by separate networks, which requires a large amount of computational resources. This work proposes PillarFlowNet, a new approach for low-latency and high-precision LiDAR scene flow estimation and object detection based on a single network that achieves real-time performance.

**Note1:** 
The goal of the article is the multi-task learning problem of 3D object detection and scene flow estimation using LiDAR data in a single deep network.3D scene flow is a point of interest for deeper understanding, and its definition associates displacement vectors to each point in a point cloud and propagates them forward to the corresponding location in a continuous point cloud. Estimating 3D scene flow using LiDAR data is a complex task because of the inherent sparsity of measured points in 3D space, where there is almost no one-to-one correspondence of point orientations in two consecutive point clouds. The scene flow must be inferred from the potential motion of objects in the scene. There is still little research in this area, and research points in this area can be dug deeper.

**Note2:** 
The highlight of the paper is the use of a single network for simultaneous point cloud object detection and scene flow estimation. Networks in previous work relied on computing expensive 3D convolutions to find correspondences in the spatial and temporal domains, which makes it too slow for real-time applications. The paper proposes that the main feature of the network is a pillar-dependent feature representation combined with efficient 2D convolution. The increase in speed makes it the first LiDAR object detection and scene flow multitask prediction network that can run in real time. However, there is still room for improvement in its accuracy of detection and scene flow estimation.

**Note3:**
I hope the authors will release the source code for us to study.