---
title: Recent Gains from reading research papers[June 16th]
author: Tianxiong Zhang
date: '2023-06-16'
slug: recent-gains-from-reading-research-papers-June-16th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2023-06-16T20:38:32+08:00'
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
#### [1]Wang S, Che Y, Zhao H, et al. Accurate tracking, collision detection, and optimal scheduling of airport ground support equipment[J]. IEEE Internet of Things Journal, 2020, 8(1): 572-584.


The thesis aims to reduce the risk of accidents on the ramp, and its design of real-time, high-precision tracking algorithms for ground vehicles or equipment that can be informed of position and speed in time and report potential collisions between aircraft and ground targets. Specifically, the thesis develops a real-time, high-precision tracking device consisting of a real-time kinematic (RTK) unit and a heading unit for securing vehicles, and most importantly, the device can be used for baggage carts with multiple trailers and tracking accuracy to within centimeters, which is not studied in other papers.

**Note 1:** 
The main implementation of the tracking algorithm in this thesis is to install a tracking device to each section of the trailer and obtain the real-time position Pi of each trailer and its heading θi through the coordinate conversion algorithm. in addition, in order to predict potential collisions, the moving speed of the secured vehicle needs to be obtained. The approach used is the estimation of the collected position data. Since the time difference method of estimating the velocity from noisy position measurements (i.e., [x(n) - x(n-1)]/T)x(n) amplifies the noise, it uses a tracking algorithm, i.e., Markov linear tracking system, and a Kalman filter to obtain the accuracy-improved positions and estimated velocities of the trailers on the x and y axes, respectively.

**Note 2:**
The collision detection of this system focuses on the corner points on the tractor or trailer, especially on the last trailer, such as the red star position in the above figure. However, the paper only acquires the position of the corner points by coordinate transformation, and does not realize the specific conflict collision detection, in which the research can still be continued.


