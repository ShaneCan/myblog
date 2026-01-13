---
title: Recent Gains from reading research papers[July 20th]
author: Tianxiong Zhang
date: '2023-07-20'
slug: recent-gains-from-reading-research-papers-July-20th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2023-07-20T20:38:32+08:00'
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
#### [1]Fang Z, López A M. Intention recognition of pedestrians and cyclists by 2d pose estimation[J]. IEEE Transactions on Intelligent Transportation Systems, 2019, 21(11): 4773-4783.

The paper explores the use of 2D attitude estimation from monocular images as the core information to recognize the intent of pedestrians and cyclists and to solve the pedestrian crossing/non-crossing classification (C/NC) task. For cyclists, the article assumes that they obey traffic rules and use arm signals to indicate future maneuvers. For pedestrians, it is assumed that the pedestrian's walking pattern determines whether he/she has the intention to cross the street in the path of the self vehicle. The paper compares favorably to other papers of its kind, mainly complementing the detection by obtaining the effect of a noisy 2D skeleton and proposing the features that C/NC classifiers consider most relevant. It is also shown how the same approach can be used to recognize cyclist arm signals.

**Note:** 
For this type of task, the application can be extended to recognize the movements of people on the ramp by drawing on the article's selection of the 9 most stable keypoints for humans, corresponding to the legs and shoulders, since the legs perform the start-stop motion of walking, and the keypoints of the shoulders and legs give the overall body orientation. Specifically, features were computed from the selected keypoints by first normalizing the coordinates of the keypoints using a factor h proportional to the height of the pedestrian, which was determined as the vertical distance from the top to the bottom keypoint. Then, different features are computed by considering the distances and relative angles between pairs of keypoints as well as the angles of the triangles induced by the triad of keypoints (conveying redundant information). Finally, a random forest classifier can be used to perform C/NC classification by directly providing the probability of a meaningful threshold treatment.
