---
title: "Learning Innovations for State Estimation"
author: "<u>G. Kennedy</u>, J. Gao, Z. Zheyu, X. Yu, R. Mahony"
collection: publications
permalink: /2021_iros
excerpt: 
date: 2021-07-01
venue: "IEEE International Conference on Intelligent Robots and Systems (IROS)"
paperurl: 
citation:
header:
   teaser: depth_comp_thumb.png
---

<a href="http://kennege.github.io/files/iros-2021.pdf" target="_blank"><b>PDF</b></a>&emsp;
<!-- <a href="http://kennege.github.io/files/exploit.bib" target="_blank"><b>BibTex</b></a> -->

![banner](/images/depth_comp.png){:class="img-responsive"}

<b>Abstract.</b> Deep learning algorithms such as Convolutional Neural Networks (CNNs) are currently used to solve a range of robotics and computer vision problems.
These networks typically estimate the desired representation in a single forward pass and must therefore learn to converge from a wide range of initial conditions to a precise result.
This is challenging, and has led to increased interest in the development of separate refinement modules which learn to improve a given initial estimate, thus reducing the required search space.
Such modules are usually developed ad-hoc for each given application.
In this work we propose a generic innovation-based CNN.
Our CNN is implemented along with a stochastic gradient descent (SGD) algorithm to iteratively refine a given initial estimate.
The proposed approach provides a general framework for the development of refinement modules applicable to a wide range of robotics problems.
We apply this framework to object pose estimation and depth estimation and demonstrate significant improvement over the initial estimates, in the range of 4.2 - 8.1\%, for both applications.

<b>Reference:</b>
G. Kennedy, J. Gao, Z. Zheyu, X. Yu, R. Mahony, "Learning Innovations for State Estimation", IEEE International Conference on Intelligent Robots and Systems (IROS), 2021.
