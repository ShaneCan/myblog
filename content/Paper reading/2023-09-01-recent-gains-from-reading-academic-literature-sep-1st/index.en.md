---
title: Recent Gains from reading research papers[Sep 1st]
author: Tianxiong Zhang
date: '2023-09-01'
slug: recent-gains-from-reading-research-papers-Sep-1st
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2023-09-01T20:38:32+08:00'
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
#### [1]Steininger D, Kriegler A, Pointner W, et al. Towards Scene Understanding for Autonomous Operations on Airport Aprons[C]//Proceedings of the Asian Conference on Computer Vision. 2022: 147-163.

This is a work published in CVPR, which focuses on the design of a dataset for the operation of an apron field for autopilot, specializing in static and dynamic objects commonly found in the apron area. And a method for image acquisition and annotation of object instances and environmental parameters is proposed that automatically extracts a representative set of samples from a large amount of image data while minimizing the manual work required for annotation. In addition, the authors produced several dataset variants on which baseline classification and detection experiments were performed, which were used to evaluate the overall performance and robustness of the resulting model to specific environmental conditions.

**Note1:**  
The fact that the paper can be published in CVPR illustrates the scarcity and necessity of in-airport unmanned datasets. The paper is specifically based on acquiring image data by working with airports to install cameras on multiple safeguard vehicles, containing results from multiple seasons of operation on the ramp and in the logistics area. Variations in environmental conditions such as time of day, seasonal and atmospheric effects, lighting conditions, and camera-related degradation effects are also included. The labeling of the dataset focuses on multiple types of ramp vehicles and also includes other types of static and transient obstacles. From the paper, it can be said that the dataset has covered most of the scenarios within the apron, but the dataset does not seem to be publicly available and is not directly accessible.

**Note2:** 
Specific data collection methodology: recorded via Nextbase 612GW CarLog, using a resolution of 3860x2160 pixels, mounted on the inside of the windshield of two containerized delivery vehicles. One was modified to include a 90° field of view instead of using the 150° built-in lens. The majority of the data was captured in time-lapse mode at 5 fps to provide data variability that fully represents the environment. In addition, the recordings were supplemented with 30 fps sequences for future studies such as multi-target tracking.

**Note3:** 
The authors' innovation was to give the dataset an additional set of defined parameters assigned to specify and categorize environmental factors during the recording time period, as shown in the figure below. This can be learned from in future production of the dataset.
