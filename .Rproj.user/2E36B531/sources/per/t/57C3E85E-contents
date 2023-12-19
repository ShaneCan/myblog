---
title: Recent Gains from reading research papers[Dec 7th]
author: Tianxiong Zhang
date: '2023-12-07'
slug: recent-gains-from-reading-research-papers-Dec-7th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2023-12-07T20:38:32+08:00'
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
#### [1] Rosinol A, Leonard J J, Carlone L. Nerf-slam: Real-time dense monocular slam with neural radiance fields[J]. arXiv preprint arXiv:2210.13641, 2022.

The paper proposes a novel pipeline for accurate and real-time reconstruction of scenes from monocular images using geometric and photometric 3D mapping. The work leverages recent advancements in dense monocular SLAM and real-time hierarchical volume-based neural radiance fields (NeRF). Dense monocular SLAM refers to specific methods that solely utilize monocular images to provide accurate scene pose estimation and depth maps. Neural radiance fields are neural networks that model the 3D structure and appearance of a scene by modeling the radiance (light intensity) at each point in space. By combining information from dense monocular SLAM with neural radiance fields, it becomes possible to create real-time, photometrically accurate scene maps. The use of uncertainty-based depth loss helps improve the photometric and geometric accuracy of the maps by addressing the uncertainty in depth estimates provided by the dense monocular SLAM system. By considering this uncertainty, the proposed method achieves significantly better results in terms of photometric and geometric accuracy compared to competing methods, with a 179% improvement in peak signal-to-noise ratio (PSNR) and an 86% improvement in L1 depth, which is remarkable and indicates a new direction for SLAM research.

**Note1:**
The breakthrough of this work lies in proposing the first 3D scene reconstruction pipeline that combines the advantages of dense monocular SLAM and hierarchical volume-based neural radiance fields. The core idea is to use a monocular dense SLAM method to estimate camera poses and dense depth maps along with their uncertainties and utilize this information as supervision to train the NeRF scene representation. This approach constructs accurate radiance fields from the image stream without requiring pose or depth as input and operates in real-time. It achieves state-of-the-art performance on a replica dataset of monocular methods. Future work is suggested to build upon this latest research.

**Note2:** 
NeRF was initially developed for image rendering, i.e., generating an image from a given camera view. NeRF is built upon the assumption of known camera poses, but in most robotic applications, the camera poses are unknown. Consequently, more recent work applies NeRF techniques to simultaneously estimate camera poses and model the environment, known as NeRF-based SLAM.

Recent research has shown that given sufficiently good initial estimates, having a given camera view is not strictly necessary. Therefore, real-time pose-agnostic NeRF reconstruction can produce accurate 3D maps. Overall, the article leverages recent research advancements in dense monocular SLAM (Droid-SLAM), probabilistic volume fusion (Rosinol et al.), and hash-based hierarchical volume neural radiance fields (Instant-NGP) to estimate the geometry and photometry of scenes in real-time without the need for depth images or poses.

**Note3:**
The fusion of deep learning and traditional geometry is a trend in SLAM development. In the past, some modules in SLAM that relied on single-point methods have been replaced by neural networks, such as feature extraction (SuperPoint), feature matching (SuperGlue), loop closure (NetVlad), and depth estimation (MonoDepth), among others. Compared to single-point replacements, NeRF-based methods present a completely new framework that can replace traditional SLAM end-to-end, both in terms of design methodology and implementation architecture.

Compared to traditional SLAM, NeRF-based methods have the following advantages:

-Directly operate on raw pixel values without feature extraction. The error is regressed to the pixels themselves, resulting in more direct information transfer and an optimization process that yields immediate visual results.

-Both implicit and explicit map representations can be differentiable, allowing for full-dense optimization of the map (traditional SLAM typically struggles to optimize dense maps and usually only optimizes a limited number of feature points or updates the map coverage).