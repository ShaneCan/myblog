---
title: Recent Gains from reading research papers[Sep 15th]
author: Tianxiong Zhang
date: '2023-09-15'
slug: recent-gains-from-reading-research-papers-Sep-15th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2023-09-15T20:38:32+08:00'
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
#### [1]Rozsa Z, Sziranyi T. Optical Flow and Expansion Based Deep Temporal Up-Sampling of LIDAR Point Clouds[J]. Remote Sensing, 2023, 15(10): 2487.

This paper proposes a framework to generate a virtual point cloud of the radar for the current frame by using the image of the current frame of the camera and the point cloud of the previous frame of the lidar (mainly because the radar scans at a mere 5-20hz, and the image refreshes at a much faster rate, leading to temporal desynchronization between the two), making temporal upsampling of the point cloud possible. The only requirement for this system is a camera with a higher frame rate than the lidar. The general flow of the algorithm is to first utilize the optical flow estimation from the available camera frames, and second, upgrade it to a 3D scene flow by optical expansion. Subsequently, a ground plane is fitted to the previous LIDAR point cloud. Finally, the estimated scene stream is applied to the previously measured object points to generate a new point cloud.

**Note1:** 
The highlight of the paper is that previous point cloud prediction methods require five or more previous frames to generate virtual measurements, while the article requires one frame.

**Note2:** 
The paper solves the problem of sampling frequency lower than the image by generating a virtual point cloud. The virtual point cloud generation is faster and more accurate, but the static targets are not considered for the design and the ground point modeling affects the accuracy, which can be considered for improvement.

**Note3:** 
The optical flow method is also one of the points that can be improved, because the optical flow method receives a lot of influence from light changes and object occlusion, and the robustness is not good, it can be considered to use the deep learning method and neural network for trajectory prediction instead of the optical flow method, but this will lead to an increase in the amount of computation, which is a problem that still needs to be considered.


