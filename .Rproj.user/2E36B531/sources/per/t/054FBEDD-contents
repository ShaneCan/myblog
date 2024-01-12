---
title: Recent Gains from reading research papers[Jan 5th]
author: Tianxiong Zhang
date: '2024-01-05'
slug: recent-gains-from-reading-research-papers-Jan-5th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2024-01-05T20:38:32+08:00'
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
#### [1] Zhou J, Elksnis A, Fu Z, et al. MultiMap3D: A Multi-Level Semantic Perceptual Map Construction Based on SLAM and Point Cloud Detection[C]//2023 28th International Conference on Automation and Computing (ICAC). IEEE, 2023: 1-6.

This paper presents a real-time multi-level semantic map generation approach based on the recent advancements in anchor-free methods for point cloud object detection in terms of computation time and accuracy. Combining visual SLAM, ground segmentation, point cloud object detection, and data association strategies for major semantic instances, a hierarchical graph is constructed in real-time. The multi-level maps consist of four layers: three-dimensional semantic metric layer, two-dimensional semantic grid layer, object layer, and room layer. A data association strategy is designed to track object instances across multiple frames and maintain a database of tracked objects. The paper also proposes a simple and effective method for room recognition using the SVC algorithm. Options for generating and blending training data are explored to address the limited real-world data for training SVC.

**Note1:**
Few researchers in current studies have combined geometric reconstruction (such as SLAM/SFM and multi-view stereo) with deep learning-based semantic segmentation or object detection methods to build multi-level semantic maps. Navigation and path planning using metric maps alone lead to significant storage and redundancy issues. Therefore, it is necessary to integrate low-level obstacle avoidance and motion planning with high-level task planning by constructing maps with multi-level semantic information. This allows robots to quickly and efficiently capture different abstraction levels of reality and perform more complex tasks in indoor scenarios.

**Note2:**
The highlight of this work lies in the fusion of target detection with SLAM, generating semantic SLAM maps with 3D object detection boxes. Additionally, it delves into understanding how the preprocessing of raw 3D data affects the performance of laser odometry. However, the method has not been tested in outdoor scenarios yet, and future work involves optimizing pose estimation and extending the algorithm to apron usage.