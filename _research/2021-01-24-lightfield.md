---
title: 'Lightfield Photography'
permalink: /posts/lightfield/
excerpt_separator: <!--more-->
tags:
  - lightfield
  - photography
header:
   teaser: lightfield.png
---

The light field is the full description of light as it travels in all directions through space around us. 
It can be thought of as being made up of infinitely many light ray vectors, each with a direction of propagation and a magnitude that is proportional to their intensity. 
As humans, we view the world by interpreting the intensity and frequency of the subset of light rays that intersect our eyes. 
However, our eyes, just like standard cameras, are incapable of recording the direction of these light rays.
Recording the direction of these light rays allows for the light field to be fully defined at a given location.
In this post I provide an introduction to the lightfield and lightfield photography.

<!--more-->
# Light

Visible light propagates through space as part of the electromagnetic spectrum.
This part of the electromagnetic spectrum incorporates frequencies of between 430 and 700 Terahertz (THz), and contains within it all the colours that we see. These colours are visible to us due to the different frequencies at which light is reflected and absorbed by different objects. 
Light can also be deflected when it passes through an object, in a phenomenon known as refraction. 
It is refraction that allows light to be focused by a lens onto an image sensor.

# The Image Sensor
Image sensors come in two main varieties: Complementary Metal Oxide Semiconductor (CMOS), or the older Charge-Coupled Devices (CCD). 
When the image sensor is exposed, photons hit the photoactive areas on the sensor, called ‘pixels’, and an electrical charge is produced. 
It is the differing ways in which these charges are produced that differentiates CMOS and CCD sensors. 
Placing a filter, such as a Bayer filter, over the pixels on a sensor allows the frequency of light to dictate the amount of electric charge produced. 
Pixels can therefore be used to determine the intensity of different colours within a scene. 
Intensity is often also referred to as ‘irradiance’ and is a measure of power per unit area. 
These filters comprise of patterns of colour filters that allow different wavelengths of light through (see Figure 1). 
The missing information between consecutive colour filters of the same type is added to the scene via interpolation to create the final image.

![wheel](/images/bayes.png){:class="img-responsive"} 
<small><i>Fig 1. Bayer filter above image sensor pixels.</i></small>

# Cameras
In a standard camera, light is focused by a lens, through a filter, onto an image sensor. 
When this sensor is exposed the pixel responses are integrated over the exposure duration. 
The image that is produced has a single plane of focus that is dictated by the distance between the lens and the sensor (the focal length). 
Parts of the scene that are not within the plane of focus are recorded by the sensor as unfocused, blurry spots. 
This is because light rays propagating from these depths are not precisely focused on to the sensor by the lens. 
However, capturing the full light field, rather than just the summation of photon responses, allows for light rays at all depths to be focused on to the sensor. 

# The Light Field
While the true behaviour of light is complicated, its movement through space is usually simplified to a light ray vector for image-based applications. 
This simplification allows the direction and intensity of light rays to be conserved while the more complicated properties of light are ignored. 
Each light ray is the result of reflection of light by a body, and contains within it a projection of that body. 
This projection can be captured by a camera at a given location. 
For example, a pin-hole camera works by capturing a small subset of these rays, and will capture a different subset (and thus a different perspective) depending on its location relative to the body (see Figure 2). 
It is therefore not only the intensity of light rays, but also their orientation and direction (i.e. their angle of incidence) that dictates the resultant image.
It follows that to fully describe the behaviour of light as it flows through a camera lens to the image sensor, one must quantify not only the intensity of the light rays in this volume, but also their orientation and direction. 
This full description of light rays is what is known as the light field. 
The light field can therefore be thought of as the infinite collection of light ray vectors, each with a magnitude proportional to their intensity, that exists around us. 
The question that arises at this point is, how many dimensions are required to fully define light ray vectors?

![wheel](/images/pinhole.png){:class="img-responsive"} 
<small><i>Fig 1. Light rays reflecting off a body and being captured by a pin-hole camera.</i></small>

<!--

# Lightfield Photography

Light field photography allows the direction of light rays to be captured. 
This means that a higher dimensional representation of light is captured by a light field camera compared to a standard camera. Light field cameras therefore provide a new, more detailed way of sensing light in an environment. 
This dense sensor information is already being applied to existing applications within the research fields of robotics and computer vision. 
Such applications include odometry, depth mapping, 3D image reconstruction, and image filtering. 
By capturing more information about a scene, these applications are able to gain more information from a single
image. 
For example, 3D image reconstruction requires multiple images of a scene to be taken taken from different, known camera poses. This method is referred to as ‘stereo vision’. 
The directional dimensions that are added by taking multiple standard images are captured in a single light field image.
 -->


