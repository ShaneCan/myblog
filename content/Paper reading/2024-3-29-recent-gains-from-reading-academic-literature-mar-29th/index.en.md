---
title: Recent Gains from reading research papers[Mar 29th]
author: Tianxiong Zhang
date: '2024-03-29'
slug: recent-gains-from-reading-research-papers-Mar-29th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2024-03-29T20:38:32+08:00'
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
#### [1] Charatan D, Li S, Tagliasacchi A, et al. pixelsplat: 3d gaussian splats from image pairs for scalable generalizable 3d reconstruction[J]. arXiv preprint arXiv:2312.12337, 2023.

The paper presents the pixelSplat3D reconstruction method, capable of reconstructing a 3D radiance field parameterized by 3D Gaussian primitives from a pair of images. The main features of this method include the ability to achieve real-time rendering and memory-efficient training, as well as rapid 3D reconstruction during inference. pixelSplat overcomes local minima issues by predicting a dense probability distribution of 3D positions and sampling Gaussian means from this distribution. Additionally, the method employs a reparameterization trick to make the sampling operation differentiable, thus allowing gradients to backpropagate through the Gaussian splatting representation.

**Note 1:**
In real-world datasets, due to the limitations of Structure from Motion (SfM) software, the reconstructed camera poses only have an arbitrary scale factor, leading to scale ambiguity issues. The paper addresses this by designing a multi-view epipolar transformer that can reliably infer the scale factor for each scene. This method finds correspondences between two reference views and combines them with depth values encoded with positional information, enabling the model to correctly predict the position of each Gaussian primitive without knowing the global scale.

**Note 2:**
In generalized 3D reconstruction, directly optimizing Gaussian primitive parameters through gradient descent can easily fall into local minima. To address this problem, pixelSplat proposes a novel parameterization approach that predicts the probability distribution of Gaussian positions instead of directly predicting depth values, and makes the sampling operation differentiable through reparameterization. This way, as gradient descent increases the opacity of a Gaussian at a certain 3D location, the model also increases the probability that the location will be sampled again in the future, thus avoiding local minima while maintaining gradient flow.

**Note 3:**
The paper primarily addresses the problem of 3D reconstruction from a pair of images. Future research could explore how to extend this method to a wider range of applications, such as reconstruction from multiple viewpoints or using different types of image data. Moreover, there may still be certain limitations when dealing with complex scenes and objects rich in detail. Future work could further improve the accuracy and detail of 3D reconstruction by enhancing the network structure, introducing more advanced prior knowledge, or combining other types of sensor data.

