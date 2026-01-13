---
title: Recent Gains from reading research papers[May 12th]
author: Tianxiong Zhang
date: '2023-05-012'
slug: recent-gains-from-reading-research-papers-may-12th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2023-05-12T20:38:32+08:00'
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
#### [1]Xu Q, Xu ZW, Du XF. QR code based visual navigation AGV system[J]. Sensors and Microsystems,2019,38(02):83-86+90.DOI:10.13873/j.1000-9787(2019)02-0083-04.

At present, there are three types of AGV navigation methods: magnetic navigation, visual navigation and laser navigation. Among them, magnetic navigation technology is mature and most used in the AGV industry, which is mainly applied to the magnetic line strip in the factory area, with high equipment erection cost and fixed operation line. Visual navigation usually adopts image processing technology as the core technology of AGV navigation, which has a high degree of autonomy, and it is more advantageous in terms of positioning accuracy and production cost. Therefore, this article designs a visual navigation system that can autonomously locate with high accuracy by using QR code, a quick response code, and an on-board camera to form the visual navigation component of AGVs.

**Note 1:** 
Extended to the apron unmanned citation scenario, consider whether the above approach can be borrowed. For the method of posting magnetic line strips in the field, which has the problem of fixed routes, and different aircraft docking locations, this method is obviously not suitable for apron operation. Considering the laser Slam navigation method, it can only be applied to indoor scenes and cannot be used to build maps for outdoor scenes. Therefore, the visual method is the most suitable.

**Note 2:**
The most mainstream method of the visual method is to paste QR code on the ground, i.e., by pasting QR code on the apron surface, in order to achieve autonomous navigation of the secured vehicles. The QR code posted in the apron can store the coordinate information of each location in the apron. Each QR code label contains a QR code code information and coordinate point (x,y) location information. When the protection vehicle passes the QR code in the apron, the information of the point can be read quickly by the camera to locate and correct the path taken, so as to realize the requirement of automatic guidance control of the self-driving protection vehicle according to the predetermined path. The technical details of this method still need to be studied in depth.






