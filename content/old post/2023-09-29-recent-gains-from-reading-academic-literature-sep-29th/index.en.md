---
title: Recent Gains from reading research papers[Sep 29th]
author: Tianxiong Zhang
date: '2023-09-29'
slug: recent-gains-from-reading-research-papers-Sep-29th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2023-09-29T20:38:32+08:00'
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
#### [1]Rozsa Z, Sziranyi T. Object detection from a few LIDAR scanning planes[J]. IEEE Transactions on Intelligent Vehicles, 2019, 4(4): 548-560.

This paper presents a LiDAR identification method based on a small number of detection planes. It is also applicable to the current single line LiDAR on ROS carts. Current research has focused on target detection for close range LiDAR, typically targeting objects within a range of 10-20 m and no more than 30 m. Surface features of 3D LiDAR are not present in strongly discontinuous point cloud segments at greater distances and greater distances. The significance of this work is that the processing range can be increased to better support processing in higher speed scenes. Currently LiDAR sensors can still be used to detect points at greater distances, but there is no available surface information. So this work proposes a solution that utilizes the available information as much as possible.

**Note:** 
In high-speed autonomous driving car applications, a robust solution is needed to recognize far-field outdoor objects. Even in the best case (Velodyne VLS-1285 with very high vertical resolution), at a range of 150 meters (a 130 km/h vehicle on a highway approaching an object in about 4 seconds), LIDAR cannot see an object 1.5 meters high in more than 5 planes, and it can only see interruptions of it. The paper also mentions the difference between AGVs and self-driving vehicles in that AGVs are slower, whereas autonomous driving vehicles need to consider safe operation at faster speeds. When looking at autonomous driving in road traffic, it is possible that focusing more on AGV operation would come up with better ideas.