---
title: Master's thesis defense[May 16, 2024]
author: Tianxiong Zhang
date: '2024-05-16'
slug: Master's thesis defense
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2024-05-16T20:38:32+08:00'
featured: no
draft: no
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/CpkOjOcXdUY)'
  focal_point: ""
  placement: 2
  preview_only: false
projects: []
summary: "Title:Research on computer vision based movement conflict detection in aircraft stand"
---
# Master's Thesis Title: Research on computer vision-based movement conflict detection in aircraft stand

## Abstract:
Ensuring the safety of airport surface operations necessitates vigilant monitoring of aircraft and vehicle activities at the aircraft stand. This thesis grounded in computer vision technology, for the detection of aircraft's key components within the stand and the identification of potential conflicts both among aircraft and between aircraft and Ground Support Equipments (GSEs).

**(1)** A comparative analysis of video imagery-based aircraft key components detection methods was conducted. An aircraft key components detection dataset within the aircraft stand area was established. The efficacy of conventional image processing algorithms was benchmarked against advanced deep learning-based networks, such as Mask-RCNN for instance segmentation, and ResNet and HRNet for key point detection. This analysis yielded the most effective algorithmic network for key point detection within the aircraft stand.

**(2)** Optimization of the aircraft keypoint detection network based on video imagery was carried out. Building on the optimal algorithm, an efficient keypoint detection network, SEHRNet, was designed by improving the output feature map coordinate decoding method, incorporating depthwise separable convolution, attention mechanisms, and adding SEBottleneck modules for network optimization. Through ablation experiments and comparisons with similar networks, SEHRNet demonstrated superiority in the task of aircraft key component recognition by significantly reducing network computational complexity and parameter quantity without sacrificing algorithm accuracy.

**(3)** Development of a single aircraft key component activity conflict detection algorithm. A camera imaging coordinate conversion algorithm for fixed cameras was developed to achieve precise conversion from two-dimensional images to three-dimensional world coordinates. Based on the kinematic model of aircraft taxiing processes, conflict detection algorithms for aircraft wingtips and engine safety areas were designed, and experimental validation was conducted with an apron physical sandbox, maintaining F1-scores above 90%.

**(4)** By introducing a kinematic model of support vehicles within the stand area, safety zone delineation for multiple key components of the aircraft was completed, and a multi-key component activity conflict detection algorithm was designed. This allowed for real-time, refined perception of potential conflicts involving multiple vulnerable and costly components within the stand area and the effective integration of multi-component conflict perception. Algorithm validation showed that all safety zones achieved F1-scores above 90%, with an average F1-score of 95% and an average frame rate above 20, indicating the strong accuracy and real-time capability of the conflict determination algorithms designed in this study.

**(5)** A visualization algorithm verification software platform based on PyQt5 was developed. This software, based on video image monitoring, possesses features such as algorithm model selection, parameter setting, real-time display, as well as program operation and alarm information display, and algorithm validation was performed through this software platform. This research enhances the intelligence level and conflict warning accuracy of the aircraft stand area monitoring system, providing algorithm support for remote control towers and automated control systems.

**Key words:** Airport, Aircraft Stand, Conflict Detection, Computer Vision, Keypoint Detection
