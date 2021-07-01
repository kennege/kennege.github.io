---
title: "State Estimation for Robotic Harvesting Applications"
author: "<u>G. Kennedy</u>"
collection: publications
permalink: /masters_thesis
excerpt: 
date: 2021-03-13
paperurl: 
citation:
header:
   teaser: pose_comp.png
---

<a href="http://kennege.github.io/files/mthesis.pdf" target="_blank"><b>PDF</b></a>&emsp;

![banner](/images/pose_comp.png){:class="img-responsive"}

<b>Abstract.</b> The global population is expected to pass 9 billion by 2050, requiring ongoing improvements in food production methods. 
Robotic harvesting offers part of the solution to this challenge, and research into the use of agricultural robots (AgBots) for harvesting horticultural crops has increased over the past several decades. 
While there has been significant progress in harvesting automation for many crops, robotic systems for crops that require selective harvesting remain far from mature. 
A key roadblock for successful implementation of such systems is the need for high-speed, high-accuracy perception pipelines.

This thesis presents three projects which aim to develop techniques to enable implementation of fast, accurate robotic harvesting perception pipelines. 
These projects utilise state estimation techniques to solve common robotic harvesting perception problems.

The initial problem involves detecting, localising, and tracking green asparagus spears with the aim of selectively harvesting this crop. 
For this task the state is the location and height of each asparagus spear. 
As part of this work I also present a design for a prototype robotic platform for harvesting green asparagus.

The second application presented in this thesis is object pose estimation and refinement from a single RGB image. 
Object pose estimation is a key technique in many robotic harvesting perception systems, where it is used to determine the pose of the target crop. 
For this application a deep learning framework, titled the Innovation CNN, is developed. 
The Innovation CNN receives an image and an initial state estimate, and computes the gradient from the estimated state to the true state. 
The result is applied iteratively in a Stochastic Gradient Descent framework to refine initial pose estimates.

The third application presented in this thesis is depth estimation and refinement from a single RGB image. 
Depth estimation is regularly used in robotic harvesting applications as a means of determining crop distance/height, or as an intermediate step in computing a 3D reconstruction. 
The Innovation CNN is also applied to this problem, again using Stochastic Gradient Descent to refine the initial depth estimate.

<b>Reference:</b>
G. Kennedy, "State Estimation for Robotic Harvesting Applications", Masters thesis, 2021.

