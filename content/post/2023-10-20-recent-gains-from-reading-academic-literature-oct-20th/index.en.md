---
title: Recent Gains from reading research papers[Oct 20th]
author: Tianxiong Zhang
date: '2023-10-20'
slug: recent-gains-from-reading-research-papers-Oct-20th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2023-10-20T20:38:32+08:00'
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
#### [1] 吴飞,金圣洁,林晓琛.基于Mask R-CNN和关键点提取的抓取位姿估计方法[J].合肥工业大学学报(自然科学版),2023,46(09):1178-1184.

In this paper, a maskregion-based convolutional neural network (MaskR-CNN) and key point extraction method is proposed for the problem of arbitrary grasping position of target workpieces in the industrial field, which is scattered and stacked in the space and obscured. We use instance segmentation for the workpieces to be grasped and the non-grasped workpieces in the grasping environment, and construct the grasping target surface point cloud; we extract the key points of 3D scale-invariant features from the target surface point cloud and extract the key points of 3D corner points from the template point cloud, and use the extracted key points as the initial values of the sampling consistency initial alignment algorithm, so that the computational amount of the point cloud alignment is reduced, and we can achieve the coarse alignment between the target surface point cloud and the reference template point cloud. Then, the iterative nearest point algorithm is used for accurate alignment.

**Note1:**  
The way of extracting the surface point cloud by Mask-RCNN is relatively novel, and the ICP algorithm of iterative nearest point can greatly reduce the computation amount of point cloud alignment, and the way of realizing it is relatively simple, which can be learned from the article, especially can be applied to the scene flow estimation, and the inter-frame matching.

**Note2:** 
Mask-RCNN this instance segmentation algorithm is poor in real-time, the article did not mention the real-time problem, this aspect will be the focus of the future consideration of improvement.