---
title: Recent Gains from reading research papers[Nov 3rd]
author: Tianxiong Zhang
date: '2023-11-03'
slug: recent-gains-from-reading-research-papers-Nov-3rd
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2023-11-03T20:38:32+08:00'
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
#### [1] Hariya, Keigo, Hiroki Inoshita, Ryo Yanase, Keisuke Yoneda, and Naoki Suganuma. 2023. "ExistenceMap-PointPillars: A Multifusion Network for Robust 3D Object Detection with Object Existence Probability Map" Sensors 23, no. 20: 8367. https://doi.org/10.3390/s23208367

This paper proposes a framework "ExistMap-PointPillars", a LiDAR-camera multilevel fusion approach for 3D object recognition, which is mainly used to cope with challenging and unfavorable conditions, e.g., at night or in rainy weather.The core concept of ExistMap-PointPillars revolves around the integration of pseudo-2D maps, which depict the estimated object presence area from the fused sensor data in a probabilistic manner. The core concept revolves around the integration of pseudo-2D maps, which probabilistically depict the estimated object presence areas obtained from the fused sensor data. These maps are then merged into pseudo-images generated from 3D point clouds.

**Note1:**

**The generation of pseudo-2D maps serves the following main purposes:**

Reduce computational complexity: 3D point cloud data usually contains a large amount of information, and processing this data requires significant computational resources and time. By projecting 3D data onto a 2D plane, the complexity of the data can be greatly reduced, thus reducing computational resources and time.

Simplifying the problem: It is usually simpler to deal with problems on a 2D plane than in 3D space. 2D object detection is a problem that has been extensively studied in computer vision, with many well-established methods and algorithms available for reference and use. 3D object detection, on the other hand, is relatively new and methods and algorithms are still under development.

Effective utilization of information: Although pseudo-2D maps lose some 3D information (e.g., height), it still retains most of the important information, such as the position, shape and size of objects. In addition, by designing appropriate projection methods and feature extraction algorithms, we can encode useful 3D information into 2D maps.

Enhanced Visualization: Pseudo-2D maps can be easily visualized, which helps in understanding and parsing the data, as well as checking and debugging the algorithms.

Therefore, generating pseudo-2D maps is a commonly used technique when working with 3D data, and its can be used for in-situ vehicle detection, map construction, etc.

**Note2:**
The method has a reduced number of true detections in the outer part of the error ellipse, which may result in failure to detect actually present objects in some cases and limited recall improvement for distant objects.

**Ideas for improvement are considered as follows:**

Enhancement of object detection in the outer part of the error ellipse: including improved feature extraction and classification algorithms, or the use of more sophisticated models to deal with complex backgrounds and object shapes.

Improve the pseudo-2D map generation process: consider using different projection methods or introducing more features to improve the ability of pseudo-2D maps in representing complex 3D world information.

Introducing more modalities: e.g. millimeter-wave radar, etc. This allows objects to be detected from more angles and depths, thus improving the comprehensiveness and accuracy of the detection.
