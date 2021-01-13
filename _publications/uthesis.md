---
title: "Squeezing Video out of a Lytro Light Field Camera"
author: "<u>G. Kennedy</u>"
collection: publications
permalink: /thesis
excerpt: 
date: 2017-11-11
venue: Undergraduate thesis
paperurl: 
citation:
header:
   teaser: lytro.png
---

<a href="http://kennege.github.io/files/thesis_2017.pdf" target="_blank"><b>PDF</b></a>&emsp;

![banner](/images/lytro.png){:class="img-responsive"}

<b>Abstract.</b> Light field photography represents a new way of sensing the environment that
provides higher dimensional information than standard cameras. While standard
cameras record the intensity of all light rays that intersect their sensor, light field
cameras also record the direction of these light rays, and the intensity associated
with different directions. Many new applications of light field video are expected to
be developed in the future, as this technology matures. This thesis aims to find new
ways of using the cheapest light field camera, the Lytro Light Field Camera (called
the ‘Lytro’ in this document), to develop and test applications of light field video.
A software package called ‘Lytro Remote Shutter’ has been developed, which builds
on currently available software to provide a tool for capturing dynamic light field
data sets. These data sets have associated pose information that is obtained by
synchronising the Lytro with a Universal Robot 5 robot arm. This software is also
capable of capturing a ‘manually-triggered’ video stream of ∼0.54fps by remotely
triggering the camera in a timed loop. A 200 image data set has been captured
using this software.
This thesis also presents a conceptual design of an Extraction System that has
the potential to extract video from the Lytro. This System includes an ‘Interceptor
Printed Circuit Board’ that can physically intercept light field data en route from the
image sensor to the processor within the Lytro, and a USB-FPGA board containing
a Field-Programmable Gate Array, to be used to process the data and transfer it to
an external device. This thesis also presents a preliminary list of requirements that
this system will need to meet if it is to successfully extract video from the Lytro.

<b>Reference:</b>
G. Kennedy, "Exploiting Rigid Body Motion for SLAM in Dynamic Environments", IEEE International Conference on Robotics and Automation (ICRA), 2018.
