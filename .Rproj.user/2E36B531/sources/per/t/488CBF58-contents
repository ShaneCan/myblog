---
title: Recent Gains from reading research papers[May 3rd]
author: Tianxiong Zhang
date: '2024-05-03'
slug: recent-gains-from-reading-research-papers-May-3rd
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2024-05-03T20:38:32+08:00'
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
#### [1]Li M, Liu S, Zhou H. SGS-SLAM: Semantic Gaussian Splatting For Neural Dense SLAM[J]. arXiv preprint arXiv:2402.03246, 2024.

This paper introduces the SGS-SLAM semantic visual SLAM system, which is based on Gaussian Splatting technology and is capable of integrating appearance, geometry, and semantic features through multi-channel optimization. The system compensates for the deficiencies of traditional depth and color losses in object optimization with a unique semantic feature loss and avoids reconstruction errors caused by cumulative errors through a semantic-guided keyframe selection strategy.

**Note 1:**
One of the core innovations of the article is that SGS-SLAM is the first semantic dense visual SLAM system based on a 3D Gaussian representation. It utilizes 2D semantic maps to learn a 3D semantic representation characterized by Gaussians, providing high-fidelity reconstruction and optimal segmentation accuracy compared to previous methods based on NeRF.

**Note 2:**
Another innovation of the article is the adoption of a multi-channel parameter optimization strategy, where appearance, geometry, and semantic signals jointly contribute to camera tracking and scene reconstruction. During the tracking phase, these different channels are used for keyframe selection, focusing on actively identifying objects seen early in the trajectory, thus achieving efficient and high-quality map reconstruction.

**Note 3:**
Due to the nature of the 3D Gaussian representation, geometric information not observed from multiple views in the trajectory will inevitably be missing, which may result in holes when performing scene operations such as object removal or transformation. This challenge, caused by the characteristics of the 3D Gaussian representation itself, requires future research to address the issue of unobserved geometric information using 3D geometric priors or scene repair techniques to improve the completeness of the scene representation.