---
title: Recent Gains from reading research papers[Jan 12th]
author: Tianxiong Zhang
date: '2024-01-12'
slug: recent-gains-from-reading-research-papers-Jan-12th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2024-01-12T20:38:32+08:00'
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
#### [1] Doherty K, Fourie D, Leonard J. Multimodal semantic slam with probabilistic data association[C]//2019 international conference on robotics and automation (ICRA). IEEE, 2019: 2419-2425.

Semantic SLAM problems can be decomposed into discrete inference problems: determining object class labels and measurement-landmark correspondences (data association problems), as well as continuous inference problems: obtaining the robot pose and object position set in the environment. However, under fuzzy data association, this is often a non-Gaussian inference problem, while most previous work has focused on Gaussian inference. The paper proposes a solution by representing hypotheses as multiple modes of an equivalent non-Gaussian sensor model. Then, non-parametric belief propagation is used to solve the resulting non-Gaussian inference problem.

**Note1:**
The innovation of the paper is mainly reflected in the introduction of multi-modal sensor models. The paper proposes a new method that represents hypotheses of data association as multiple modes of an equivalent non-Gaussian sensor model, which can better handle SLAM problems in non-Gaussian environments. In addition, to address non-Gaussian inference problems, the paper adopts non-parametric belief propagation. This method can effectively approximate non-Gaussian posterior, dealing with the uncertainty of complex data association and landmark categories.

**Note2:**
Although the proposed method can handle uncertain associations, it relies on hard decisions when adding new landmarks. Representing this uncertainty is an important step more closely integrating data association and SLAM problems. Furthermore, while the paper presents a method for handling complex data association, the computational cost of calculating association probabilities may be large. Future work could explore solutions to this computational complexity issue, such as using Dirichlet process priors or approximate matrix permanents. The paper assumes a simple geometric model, focusing on comparing data association methods. Another future direction is to apply new geometric representations, such as quadrics, to further improve the performance and accuracy of SLAM.