---
title: Recent Gains from reading research papers[Dec 1st]
author: Tianxiong Zhang
date: '2023-12-01'
slug: recent-gains-from-reading-research-papers-Dec-1st
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2023-12-01T20:38:32+08:00'
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
#### [1] Li R, Li S J, Chen X, et al. TFNet: Exploiting Temporal Cues for Fast and Accurate LiDAR Semantic Segmentation[J]. arXiv preprint arXiv:2309.07849, 2023.

The paper presents a distance-image-based LiDAR semantic segmentation method that utilizes temporal information to address the "many-to-one" problem caused by the limited horizontal and vertical angular resolution of distance images. This problem can result in approximately 20% of 3D points being occluded, rendering the LiDAR semantic segmentation unable to accurately and robustly understand the surrounding environment. Specifically, the article combines a temporal fusion layer to extract useful information from previous scans and integrate it with the current scan. Then, a post-processing technique based on maximum voting is designed to correct erroneous predictions, particularly those caused by the "many-to-one" problem.

**Note1:**
The so-called "many-to-one" problem refers to the influence of boundary blurring effects on the range view representation. The main cause of this problem is the limited horizontal and vertical angular resolution: when these points share the same vertical and horizontal angles, multiple points will be projected onto the same range image pixel. Handling such issues should be considered in subsequent work.

**Note2:**
The highlight of this work lies in the incorporation of temporal information in segmentation or detection, inspired by human visual perception. Temporal information is crucial for understanding object motion and identifying occlusions. By combining temporal information, severely occluded points can be captured from adjacent range image scans. The post-processing during the inference stage can also benefit from this approach. The article proposes a post-processing scheme based on maximum voting, which effectively leverages predictions from past frames.