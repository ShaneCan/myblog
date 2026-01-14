---
title: Recent Gains from reading research papers[Sep 8th]
author: Tianxiong Zhang
date: '2023-09-08'
slug: recent-gains-from-reading-research-papers-Sep-8th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2023-09-08T20:38:32+08:00'
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
#### [1] Rózsa Z, Golarits M, Szirányi T. Water Hazard Depth Estimation for Safe Navigation of Intelligent Vehicles[C]//VEHITS. 2021: 90-99.

This paper presents a method for providing water hazard information to surface vehicles. The method does not require any constraints on camera motion or specific sensors and allows determining the 3D coordinates of underwater surface points in a least squares sense.Based on the theory of multi-view geometry and basic point cloud processing techniques, the method utilizes the principle of refraction to detect underwater hazards on the basis of matching points, estimating their surfaces and calculating the true depths of underwater shapes. The method helps to improve vehicle intelligence through water hazard depth estimation in both on-road and off-road situations.

**Note1:** 
The paper proposes a new method for estimating water depth with binocular camera. The binocular camera allows the problem to be simplified and the scene reconstructed while solving the problem of detecting hazards in a timely manner at a distance and estimating the underwater depth at a close distance. As the 3D environmental reconstruction of the scene continues, segmenting the water hazard area in just one image is sufficient to mark the hazardous area in 3D.

**Note2:** 
This paper applies the devised method to the autonomous driving of ground vehicles in off-road or road pothole environments, however, it is also possible to extend this method to other vehicles, intelligent systems, for example, it can be applied to UAVs in terms of terrain detection, for water depth mapping or for search and rescue missions in case of flooding disasters.

The advantage of the method proposed in the paper is that there is no restriction on the camera attitude during the detection process and no additional or specific sensors are required. The innovation lies in the fact that the paper proposes a calibration solution that defines the vehicle and camera poses in a universal coordinate system, which has never been done before.
