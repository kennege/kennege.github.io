---
title: 'Asparagus Harvesting Robot'
permalink: /projects/asparagus-harvester/
excerpt_separator: <!--more-->
author_profile: true
tags:
  - harvesting
  - robot
  - vision
header:
   teaser: AsparagusBot_thumb.png
---

I spent a year working as a Research Assistant with the Australian Centre for Robotic Vision at the Australian National University.
During this time my main project involved the development of a prototype robotic harvester for green asparagus.
My role involved developing a vision system that would enable the robotic to detect and localise asparagus spears that were ready for harvest.

<!--more-->

# Marketing Material

<iframe src="/files/Flyer_RoboticHarvesting.pdf" width="150%" height="500" frameborder="no" border="0" marginwidth="0" marginheight="0"></iframe>
<small><i>Flyer.</i></small>

<iframe src="/files/TechSummary_RoboticHarvesting.pdf" width="150%" height="500" frameborder="no" border="0" marginwidth="0" marginheight="0"></iframe>
<small><i>Technical Summary.</i></small>


# Project Overview
Our goal was to develop a tractor-mountable green asparagus harvesting robot that operated at comparable speeds to human labour.

![](/images/AsparagusBot.png){:class="img-responsive"}
<small><i>Prototype Robotic Harvester. Courtesy of Alex Martin, ANU.</i></small>

We believed that a key to adoption of robotic harvesting technology was the simplicity with which it could be integrated into existing farm operations.
For this reason we considered high speed to be a key design requirement.
We therefore developed a vision system that relied on simple, robust algorithms that allowed for high speed data processing.
We also developed a novel `ballistic cut-and-throw' harvesting technique that allowed for harvesting of multiple asparagus spears per second. 



# Perception System

We collaborated with a local farm to trial our perception system.

![farm](/images/farm.png){:class="img-responsive"} 
<small><i>Fig 1. On-farm data capture.</i></small>

We then built a camera system and mounting platform in-lab to allow for prototyping of the vision system.

![farm](/images/inlab.jpg){:class="img-responsive"} 
<small><i>Fig 2. In-lab prototyping.</i></small>

Our vision system was designed to operate at high speeds, and was therefore based on combining simple algorithms, including homography projection, line fitting, and Kalman filtering. 

![](/images/initialPipeline.svg){:class="img-responsive"}
<small><i>Prototype Perception Pipeline.</i></small>

# Project Update
Unfortunately due to a variety of circumstances this project finished in 2019, before a complete prototype could be produced.
