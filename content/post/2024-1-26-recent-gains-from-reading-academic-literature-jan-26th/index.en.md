---
title: Recent Gains from reading research papers[Jan 26th]
author: Tianxiong Zhang
date: '2024-01-26'
slug: recent-gains-from-reading-research-papers-Jan-26th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2024-01-26T20:38:32+08:00'
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
#### [1] Nair G B, Daga S, Sajnani R, et al. Multi-object monocular SLAM for dynamic environments[C]//2020 IEEE Intelligent Vehicles Symposium (IV). IEEE, 2020: 651-657.

The paper addresses the issue of multi-object SLAM (Simultaneous Localization and Mapping) using a monocular camera. "Multi-object" signifies that the algorithm is capable of tracking both the camera's motion and the movement of other dynamic entities within the scene. A typical challenge in dynamic environments is the unobservability problem, which refers to the impossibility of triangulating moving objects explicitly from a moving monocular camera. Existing solutions suffer from relative scale ambiguity, meaning that there is an infinite number of solutions for each pair of movements within the scene. The innovation of this paper lies in its approach to resolving this issue by leveraging monocular metric, advances in deep learning, and category-level shape estimation. The paper proposes a multi-pose graph optimization formulation to address the ambiguities associated with the involved relative and absolute scale factors.

**Note1:**
The novelty of this paper is the introduction of a multi-object monocular SLAM system for dynamic environments, which is the first practical system of its kind. It can perform dynamic multi-object tracking and self-localization within a unified framework. By utilizing advances in monocular metric and category-level shape estimation through deep learning, the paper resolves the issue of relative scale ambiguity present in dynamic scenes. Category-level shape estimation is a method worth emulating in future research.

**Note2:**
The algorithm of the article may not accurately locate keypoints for objects at a greater distance, which could affect the overall performance of the system. Improving the detection and tracking of distant objects could be a direction for future work. Moreover, the current implementation may not be suitable for applications requiring real-time responses, such as autonomous driving. Further optimization of the algorithm to increase processing speed could be an important direction for improvement. Although the current method has made some progress in resolving scale ambiguity, there is still room for further in-depth research in this field, especially under various types of scenes and conditions.