---
title: Recent Gains from reading research papers[Mar 1st]
author: Tianxiong Zhang
date: '2024-03-01'
slug: recent-gains-from-reading-research-papers-Mar-1st
categories:
  - Essay
tags:
  - Deep Learning
subtitle: ''
summary: ''
authors: []
lastmod: '2024-03-01T20:38:32+08:00'
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
#### [1]  Liu Y, Zhang K, Li Y, et al. Sora: A Review on Background, Technology, Limitations, and Opportunities of Large Vision Models[J]. arXiv preprint arXiv:2402.17177, 2024.

This paper provides a comprehensive review of Sora, a text-to-video generative AI model released by OpenAI. Sora has the capability to create videos of scenes that are either realistic or imagined based on textual instructions, demonstrating potential in simulating the physical world. The paper discusses in detail the background of Sora, its underlying technologies, applications, challenges faced, and future directions for development, drawing on publicly available technical reports and reverse engineering.

**Note1:**
To effectively process videos of varying resolutions and frame rates, Sora compresses videos into a low-dimensional latent space and then decomposes them into spacetime patches. These patches function analogously to tokens in language models, providing Sora with detailed visual phrases for video construction. Moreover, Sora employs a video compression network, or visual encoder, to reduce the dimensionality of input data, particularly raw videos. This network, based on Variational Autoencoders (VAE) or its variants like Vector Quantized Variational Autoencoder (VQ-VAE), transforms video frames into fixed-size patches, which are then encoded into the latent space. This allows the model to handle videos of different resolutions and frame rates. By compressing videos into latent space representations and then extracting a series of latent spacetime patches, these patches encapsulate the visual appearance and motion dynamics over short time spans. These patches are subsequently used to generate videos through a diffusion transformer model. During training, Sora may employ a cascading diffusion model architecture, which includes a base model and multiple spacetime refinement models. This architecture enables the model to enhance the quality and frame rate of videos through cascading refinement while maintaining high resolution.

**Note2:**
SORA currently also faces some limitations that need improvement. Sora may struggle with understanding textual instructions regarding the placement or arrangement of objects and characters, which can lead to generated videos that do not match the expected spatial layout and temporal sequence. Additionally, the model may insert irrelevant elements when dealing with complex scenes containing multiple characters or elements, thereby altering the original composition and atmosphere of the scene. When simulating complex scenarios, Sora might not accurately handle physical principles such as interactions between objects, kinematics, and dynamics. This could result in generated videos with flaws in physical authenticity, such as unnatural object deformations or incorrect physical interactions. These are challenges that we need to overcome in subsequent developments.