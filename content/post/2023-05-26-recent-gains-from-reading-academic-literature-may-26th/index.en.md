---
title: Recent Gains from reading research paper[May 26th]
author: Tianxiong Zhang
date: '2023-05-26'
slug: recent-gains-from-reading-research-paper-may-26th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2023-05-26T20:38:32+08:00'
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
#### [1] Brassel H, Zouhar A, Fricke H. 3D Modeling of the airport environment for fast and accurate LiDAR semantic segmentation of apron operations[C]//2020 AIAA/IEEE 39th Digital Avionics Systems Conference (DASC). IEEE, 2020: 1-10.
#### [2] Braßel H, Zouhar A, Fricke H. Adaptive point sampling for LiDAR-based detection and tracking of fast-moving vehicles using a virtual airport environment[J].

The above-mentioned papers propose a combination of LiDAR with target detection and tracking, and semantic segmentation algorithms, respectively, to achieve surveillance tasks on non-collaborative objects. The first paper focuses on fast and accurate LIDAR semantic segmentation in the apron. The main reasons for less research in this area are the dependence of model building on large-scale datasets and the tedious point-by-point annotation of 3D point clouds. Therefore, the paper builds simulated datasets and uses a virtual airport environment with integrated LiDAR sensor models to generate synthetic training data for the ramp. In addition the model identifies aircraft arrival/departure gates, high poles, airport buildings and ground planes. And the second one proposes a method for real-time detection and tracking of fast moving objects on the ramp in LIDAR scanning based on the study of semantic segmentation of airport scenes. The method integrates the newly generated point cloud into the Kalman filter by selecting feature points as a function of the velocity and distance of the moving target from the sensor.

**Note 1:** 
Combining the above two papers shows the importance of simulated datasets in the face of unavailability of field data. A major advantage of the simulated dataset is the ease of obtaining accurate data for each time point at each location, which facilitates the verification of the accuracy of the proposed model. In addition some validations related to ramp operations can be carried out in simulated scenarios, combined with digital twins.

**Note 2:**
Simulation scenarios can be built with CAD and 3D models can be created based on publicly available ground views such as OpenStreetMap. However, freely available data sources usually provide only incomplete 3D information (e.g. height) and less detail. So building a simulation dataset also requires the collection of real data to ensure the match with reality. As in the above paper, detailed construction drawings provided directly by the airport and measurements from real LiDAR scans of the ramp were used to build the scenario.






