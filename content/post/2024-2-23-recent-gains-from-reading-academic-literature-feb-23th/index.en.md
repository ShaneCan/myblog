---
title: Recent Gains from reading research papers[Feb 23th]
author: Tianxiong Zhang
date: '2024-02-23'
slug: recent-gains-from-reading-research-papers-Feb-23th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2024-02-23T20:38:32+08:00'
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
#### [1] Tian R, Zhang Y, Feng Y, et al. Accurate and robust object SLAM with 3D quadric landmark reconstruction in outdoors[J]. IEEE Robotics and Automation Letters, 2021, 7(2): 1534-1541.

Object-oriented SLAM is a cutting-edge technology in the fields of autonomous driving and robotics. This paper introduces a stereo vision SLAM system with a robust quadratic landmark representation method. The system comprises four components: deep learning-based detection, quadratic landmark initialization, object data association, and object pose optimization. SLAM algorithms based on quadratic surfaces always face observation-related challenges and are sensitive to observation noise, which limits their application in outdoor scenes. To address this issue, the paper proposes a quadratic initialization method based on a quadratic parameter separation approach, enhancing robustness to observation noise. An adequate object data association algorithm and object-oriented optimization with multiple cues enable highly accurate object pose estimation and robustness to local observations.

**Note1:**
The innovation of this paper lies in: 1. The introduction of an algorithm based on Separating Quadric Parameters (SQP) for the initialization of 3D ellipsoidal landmarks. This method independently estimates the translation and yaw rotation of the ellipsoid center, improving robustness to observation noise. 2. The adoption of a novel Object Data Association (ODA) algorithm that combines semantic inlier distribution, motion prediction based on Kalman filtering, and ellipsoidal projection to achieve precise data association. 3. The implementation of a real-time stereo vision SLAM system that utilizes precise and robust ellipsoids to represent objects, aiming to build an object-oriented and semantically enhanced map for outdoor navigation.

**Note2:**
The accuracy of data association in scenes with dynamic objects, such as moving vehicles and pedestrians, may require further improvement to prevent incorrect object associations leading to inaccurate ellipsoid initialization. Moreover, there may be room for enhancement in the system's real-time performance and computational efficiency, especially when dealing with large-scale or complex scenes.