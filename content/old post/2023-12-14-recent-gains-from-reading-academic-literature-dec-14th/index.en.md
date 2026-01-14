---
title: Recent Gains from reading research papers[Dec 14th]
author: Tianxiong Zhang
date: '2023-12-14'
slug: recent-gains-from-reading-research-papers-Dec-14th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2023-12-14T20:38:32+08:00'
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
#### [1] Moreno F M, Guindel C, Armingol J M, et al. Study of the Effect of Exploiting 3D Semantic Segmentation in LiDAR Odometry[J]. Applied Sciences, 2020, 10(16): 5657.

The paper investigates how preprocessing point clouds using 3D semantic segmentation affects the performance of laser odometry in terms of distance measurement. It analyzes the estimated trajectories when filtering the raw data with semantic information. Different filtering configurations are tested: raw (original point cloud), dynamic (removing dynamic obstacles from the point cloud), dynamic vehicles (removing vehicles), long-range (removing distant points), ground (removing ground points), and structural (keeping only structural and object points in the point cloud). The conclusions drawn from this work are significant for improving the efficiency of laser odometry algorithms in various scenarios.

**Note1:**
The main contribution of the paper is to gain insights into how preprocessing of raw 3D data affects the performance of laser odometry. This analysis specifically focuses on a state-of-the-art method called LOAM, which is a high-performance technique that utilizes only laser scanner information and serves as the basis for many literature works.

**Note2:**
The highlight of this work lies in exploring the behavior of laser odometry by proposing six different input configurations. For each configuration, a set of newly filtered data is generated and provided to the odometry algorithm for evaluation. The experimental results confirm the effectiveness of preprocessing the data before inputting it into the localization algorithm. Furthermore, the type of driving environment has a decisive impact on the applicability of each filtering method. 