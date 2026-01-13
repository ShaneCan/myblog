---
title: Recent Gains from reading research papers[July 6th]
author: Tianxiong Zhang
date: '2023-07-06'
slug: recent-gains-from-reading-research-papers-July-6th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2023-07-06T20:38:32+08:00'
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
#### [1]Xu J, Ding M, Zhang Z Z, et al. Vision-Based Automatic Collection of Nodes of In/Off Block and Docking/Undocking in Aircraft Turnaround[J]. Applied Sciences, 2023, 13(13): 7832.

The paper is based on a target detection algorithm to automatically recognize aircraft docking and push-off, and record the corresponding safeguard event node time. It consists of two modules, which are preprocessing module and key node collection module. The preprocessing module extracts spatio-temporal information from the airport field; the key node collection module designs the interaction of single target nodes and dual target nodes represented by docking passenger elevator trucks and evacuation of passenger elevator trucks, and designs the collection methods of two kinds of key nodes. The framework can replace the manual recording methods that are routinely used at present.

**Note 1:**

The dataset of this thesis is two neighboring aircraft positions with two cameras of different viewpoints. To solve the problem that airplanes from neighboring slots may be included in one surveillance image and cannot be correlated, the thesis sets an a priori rule. That is, by analyzing the dimensions of the aircraft at positions 734 and 939 in the image plane, it is found that the width or height of the BBOX of the aircraft at the current position is at least half of the width or height of the whole. Based on this a priori rule, the airplanes are associated by searching the bounding box of the airplane with the largest area that satisfies the above rule.


**Note 2:**

To determine the target motion stationary, the thesis uses the standard deviation of the coordinates of the center point of the bounding box in consecutive frames of a certain length from the IoU values of the previous and current bounding boxes to determine the motion state, and if the IOU is greater than a certain threshold, it is determined to be stationary.


**Note 3:**

The paper determines whether docking is complete by two conditions. One is that both the passenger elevator truck and the aircraft are at rest, and the second is that based on a specific angle of the in-flight camera, it was found that if 90% of the passenger elevator truck's BBOX overlapped with the aircraft's BBOX, the docking process was judged to be complete.

Some of the determination methods in this paper are simple, but cleverly utilize the a priori information of the position of the aircraft camera, which is worthwhile.



