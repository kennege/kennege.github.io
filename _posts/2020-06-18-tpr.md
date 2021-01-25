---
title: 'Thesis Proposal Review'
permalink: /projects/tpr/
excerpt_separator: <!--more-->
tags:
  - calibration
  - robot
  - vision
header:
   teaser: tpr.png
---

My masters program requires the submission of a thesis proposal review. 
The thesis proposal review (TPR) consists of a written report detailing the candidate’s proposed research topic and a plan for future work. 
The TPR also includes an hour-long public seminar, which is followed by audience questions and a private discussion with the supervisory panel.

<!--more-->

# Abstract
State estimation is a fundamental problem in computer vision and robotic vision.
Classical computer vision problems involve extracting all relevant information from a single image or set of images. 
Conversely in robotic vision, the images are captured in real-time and require filtering algorithms that track and update target information.
In this report I present a deep learning framework that aims to be applicable in both these scenarios. 
I introduce a novel CNN architecture, termed an ‘Innovation CNN’, that estimates the innovation (difference between current state and desired/expected state) for a system. 
The Innovation CNN can be applied in a stochastic gradient descent framework to refine/update a state estimate using standard numerical optimisation techniques. 
The Innovation CNN can also be applied in a filter algorithm to update an evolving state estimate. 
In this report I discuss the literature for online and offline state estimation that is relevant to the Innovation CNN. 
The literature review particularly focuses on the initial target problem; object pose estimation. 
I also present the formulation, network architecture, and initial results for the application of the Innovation CNN to object pose estimation. 
Finally, I outline a research plan for the remainder of my candidature.

<!-- <a href="http://kennege.github.io/files/TPR.pdf" target="_blank"><b>PDF</b></a>&emsp; -->
<a href="http://kennege.github.io/files/TPR_seminar.pptx" target="_blank"><b>Slides</b></a>&emsp;


