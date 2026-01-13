---
title: Recent Gains from reading research papers[Oct 27th]
author: Tianxiong Zhang
date: '2023-10-27'
slug: recent-gains-from-reading-research-papers-Oct-27th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2023-10-27T20:38:32+08:00'
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
#### [1]K. Yoneda, N. Ichihara, H. Kawanishi, T. Okuno, L. Cao and N. Suganuma, "Sun-Glare region recognition using Visual explanations for Traffic light detection," 2021 IEEE Intelligent Vehicles Symposium (IV), Nagoya, Japan, 2021, pp. 1464-1469, doi: 10.1109/IV48863.2021.9575631.

Recognition of traffic signals is an important task in autonomous vehicles, and extracting traffic light color information is crucial. This article develops a method to recognize sun glare regions in images using Convolutional Neural Network visual interpretation in order to address the situation where traffic lights and the sun overlap ahead and the images captured by the camera are overexposed, risking false detection. The CNN outputs an attention map using the Grad-CAM method, which can then be processed through time series to estimate the global orientation of the sun glare region. By estimating the direction of sunlight that reduces visibility such as direct sunlight and reflected light from buildings, it helps to achieve robust image recognition.

**Note1:** 
The estimated posterior probability distribution can be used not only to compute the sun direction, but also to understand the areas of reduced visibility in the current image. If the image quality is affected by the exposure, the color of the light will also change. In this case, the image quality of the captured image is affected and even the human eye may have difficulty in distinguishing the illumination color. In order to prevent false alarms in this case, we need to recognize this situation in advance and specialize it.

**Note2:** 
This author has implemented only an upstream task, we also need to integrate the algorithm with specific realities, e.g., applying it to active route planning and intersection driving position planning to avoid exposure situations, or calling algorithms that remove exposure. The algorithm can also be used to guide the sensing devices in the unmanned driving of safeguarded vehicles in the apron to encounter exposure situations.