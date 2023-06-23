---
title: Recent Gains from reading research papers[May 19th]
author: Tianxiong Zhang
date: '2023-05-19'
slug: recent-gains-from-reading-research-papers-may-19th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2023-05-19T20:38:32+08:00'
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
#### [1]Wang Zheng,Zhao Xiao,She Hongjie,Liu Honghai,Zhao Yanwei. AGV obstacle detection and obstacle avoidance based on binocular vision[J]. Computer Integrated Manufacturing Systems,2018,24(02):400-409.DOI:10.13196/j.cims.2018.02.012.

This paper proposes a binocular vision-based obstacle detection and obstacle avoidance method for AGVs. In the process of obstacle detection, an obstacle determination algorithm based on depth detection is used to determine the existence of obstacles, and then the frame difference method is used to obtain the orientation and speed information of static and dynamic obstacles. In addition, we also design obstacle avoidance strategies for different obstacles, and analyze the angle and distance deviation during the movement of AGV.

**Note 1:** 
The obstacle detection scheme of this paper, as well as its motion state detection, uses binocular vision to calculate the 3D coordinates of the image matching point in the left camera coordinate system, obtain its height distance and horizontal distance, and compare it with the set threshold to determine whether the obstacle exists, rather than using deep learning target detection method, the advantages and disadvantages of the two methods are unclear and need to be further compared.

**Note 2:**
The obstacle avoidance strategy of this article is worthy of reference, and its different obstacle avoidance strategies are set according to its state after getting the obstacle motion characteristics. For dynamic obstacles, the self-driving safeguard vehicle should continue to wait in place until the obstacle leaves; for static obstacles, the self-driving safeguard vehicle should implement the obstacle avoidance strategy and then return to the normal path.
The static obstacle avoidance strategy is as follows: first, according to the target detection algorithm to obtain the length of the obstacle located in the pixel coordinate system and the offset value compared to the boundary of the obstacle compared to the center of the vehicle, according to the camera calibration algorithm, to obtain its actual length L and offset p. According to the LIDAR to know the distance between the vehicle and the front obstacle a. According to the type of obstacles identified (two kinds of obstacles in the machine position: car, human ), the obstacle width W can be set as 5m and 0.5m respectively. secondly, if the obstacle is found to be to the right relative to the vehicle, the vehicle will avoid to the left, and vice versa.




