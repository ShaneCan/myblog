---
title: Recent Gains from reading research papers[Apr 19th]
author: Tianxiong Zhang
date: '2024-04-19'
slug: recent-gains-from-reading-research-papers-Apr-19th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2024-04-19T20:38:32+08:00'
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
#### [1] Yan G, Pi J, Guo J, et al. OASim: an Open and Adaptive Simulator based on Neural Rendering for Autonomous Driving[J]. arXiv preprint arXiv:2402.03830, 2024.

This paper proposes OASim, an open and adaptive autonomous driving simulator, which generates high-fidelity autonomous driving data based on implicit neural rendering technology. It addresses the high cost, time consumption, and safety risks associated with real-world data collection through high-quality scene reconstruction, trajectory editing, a rich library of vehicle and sensor models, and a highly customizable data generation system. OASim utilizes advanced implicit surface reconstruction and 3D Gaussian splatting techniques, combined with an interactive visualization interface, allowing users to edit and preview vehicle trajectories and sensor configurations in real-time, thereby generating customized data suitable for multiple downstream applications of autonomous driving, such as perception and planning. Additionally, OASim demonstrates its experimental results in photorealistic rendering, novel viewpoint synthesis, diverse sensor configurations, and traffic flow simulation, verifying its effectiveness and advancement in autonomous driving data generation and simulation.

**Note 1:**
One of the core innovations of the article is that OASim uses implicit neural surface reconstruction technology to achieve high-fidelity scene reconstruction. This method captures complex scene details by training a multilayer perceptron (MLP) to simulate the radiance and depth of each point in the scene, resulting in high-quality rendering outcomes.

**Note 2:**
Another innovation of the article is the provision of an interactive interface that allows users to edit the trajectories of their own vehicle and other vehicles, flexibly configure sensor suites, and preview the data generated based on the edited trajectories in real-time. This interactivity provides users with a high degree of customization ability to generate data and scenarios that meet specific needs.

**Note 3:**
Although the platform currently offers a rich library of sensor models, there may still be some types of sensors not covered. The focus is primarily on the generation of visual data, and in the future, it could explore the integration of more modal data (such as sound, temperature, etc.) to provide a more comprehensive simulation environment.
