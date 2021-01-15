---
title: 'Camera-Robot Calibration Software Package'
permalink: /projects/calibration/
excerpt_separator: <!--more-->
tags:
  - calibration
  - robot
  - vision
header:
   teaser: ur5exp_thumb.jpg
---

In 2020 I collaborated with a fellow student to develop an automated regime for calibrating a multi-camera system with a UR5 robotic arm.
The software is written in Python, and has been used successfully by members of the Australian Centre for Robotic Vision.

<!--more-->

<a href="https://github.com/kennege/ur5_multicam_calib" target="_blank"><b>Code</b></a>&emsp;
<a href="http://kennege.github.io/files/ur5doc.md" target="_blank"><b>Documentation</b></a>&emsp;
<a href="http://kennege.github.io/files/ur5calibdoc.pdf" target="_blank"><b>Formulation</b></a>&emsp;

The software is setup to automatically obtain the transformation matrices between the camera(s), the base of the robot arm, the end-effector of the robot, and also optionally the work station (table). These reference frames are illustrated below. The camera parameters (focal length, principle point, etc) are also computed and provided in the typical Intrinsic matrix format.

![acrv](/images/ur5calib.png){:class="img-responsive"} 

The software makes use of an Aruco-marker board, which is a common tool for camera calibration. 
The board is attached via a custom-made joint.
The CAD model for the joint is also provided.
Below is an illustration of the software package in action.

![acrv](/images/ur5exp.jpg){:class="img-responsive"} 



