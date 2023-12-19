---
title: Recent Gains from reading research papers[Nov 24th]
author: Tianxiong Zhang
date: '2023-11-24'
slug: recent-gains-from-reading-research-papers-Nov-24th
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2023-11-24T20:38:32+08:00'
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
#### [1] Li P, Ding S, Chen X, et al. PowerBEV: A Powerful Yet Lightweight Framework for Instance Prediction in Bird's-Eye View[J]. arXiv preprint arXiv:2306.10761, 2023.

The paper proposes an end-to-end framework, POWERBEV, for vehicle motion prediction based on bird's-eye view (BEV). The framework differs in several design choices, reducing inherent redundancies in previous methods. Firstly, POWERBEV predicts the future not through auto-regressive modeling but with parallel multi-scale modules built using lightweight 2D convolutional networks. Secondly, the article employs segmentation and centripetal inverse flows for prediction, simplifying the previous multitask objectives by eliminating redundant output patterns. Based on this output representation, a simple flow-based post-processing method is proposed, which generates more stable instance associations.

**Note1:**
Currently, multi-sensor data fusion and feature extraction on bird's-eye view (BEV) are commonly used and have achieved good results. However, there is limited research on motion prediction in this regard. Traditional prediction methods based on multi-view surround cameras rely on multitask auto-regressive settings and complex post-processing to predict future instances in a spatiotemporally consistent manner. This article deviates from this paradigm.

**Note2:**
The current primary approach to predicting vehicle motion trajectories decouples the task into separate modules. In this mode, interested objects are detected and localized through complex perception models, and associations are made across multiple frames. Then, using parameterized trajectory models, the potential future motion of these detected targets is predicted based on their past motion. However, due to the separate prediction of perception and motion models, the entire system is prone to errors in the first stage. Therefore, I personally believe that an end-to-end model design can be applied to future perception, localization, prediction, and other aspects. This approach can effectively alleviate the aforementioned issues and reduce data redundancy, presenting a feasible path forward.