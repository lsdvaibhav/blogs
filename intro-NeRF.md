---
layout: distill
title: [Introduction to NeRF]
description: [Neural Radiance Fields (NeRF) Introduction & equaltions.]
date: 2022-12-30
htmlwidgets: true

# anonymize when submitting 
authors:
  - name: Vaibhav Kharatmal
  - name: Shreeram Geedh
  - name: Shristhi Mondal

# do not fill this in until your post is accepted and you're publishing your camera-ready post!
# authors:
#   - name: Vaibhav Kharatmal
#     url: "https://linkedin/lsdvaibhav"
#     affiliations:
#       name: Braiwonders, Mumbai
#   - name: Shreeram Geedh
#     url: "https://linkedin/shreeramgeedh"
#     affiliations:
#       name: Ugam, Mumbai
#   - name: Shristhi Mondal
#     url: "https://linkedin/shristhimondal" 

# must be the exact same name as your blogpost
bibliography: 2022-12-30-intro-nerf.bib  

# Add a table of contents to your post.
#   - make sure that TOC names match the actual section names
#     for hyperlinks within the post to work correctly.
toc:
  - name: [Introduction]
  - name: [Equation]
---

Neural Radiance Fields (NeRF) is a machine learning method that was introduced in a paper published in 2020 by researchers at Stanford University and Facebook AI Research. 
It is a method for generating photorealistic 3D models of scenes from a set of 2D images.

One of the key features of NeRF is its ability to generate highly detailed 3D models with a high level of realism. 
It does this by learning a continuous 3D function that maps 2D image coordinates to 3D scene radiance. 
This allows it to generate highly detailed 3D models that capture both the appearance and the geometry of a scene.

In order to generate a 3D model using NeRF, the system is trained on a dataset of 2D images of a scene, along with the corresponding 3D geometry and lighting information. 
It then learns to predict the 3D radiance at each point in the scene, allowing it to generate a detailed 3D model of the scene.

One of the main advantages of NeRF is its ability to generate high-quality 3D models from relatively small datasets. 
This is because it uses a continuous 3D function to model the scene, rather than discrete 3D points or voxels. 
This allows it to capture fine-grained details and smooth transitions between different parts of the scene, even if those details are not present in the training data.

Overall, NeRF is a powerful and innovative machine learning method that has the potential to revolutionize the way we generate 3D models of real-world scenes. 
It has a number of applications, including computer graphics, virtual reality, and augmented reality, and it has already been used to generate some impressive results in these areas.

This equation defines the 3D radiance, L(x), at a point x in the scene as a function of the viewing direction, v, and the 2D image coordinates, u. 
The function f(x,v) is a neural network that maps the 3D position and viewing direction to the radiance at that point. The function g(u) maps the 2D image coordinates to the 3D position and viewing direction in the scene.

The term S(x) is a scalar function that encodes the surface albedo (reflectance) at each point in the scene, and the term I(x) is a scalar function that encodes the incoming lighting at each point in the scene.

Finally, the term ∫L(x')dω' is an integral over all points x' in the scene, which takes into account the contribution of light from other points in the scene to the radiance at x. 
This term is known as the volume scattering term and it helps to capture the way that light is scattered and absorbed as it travels through the scene.



Neural Radiance Fields (NeRF) has a number of potential use cases, including:

Computer graphics: NeRF can be used to generate highly detailed and photorealistic 3D models of real-world scenes, which can be used in computer graphics applications such as film, television, and video games.

Virtual reality: NeRF can be used to generate 3D models of real-world scenes that can be used in virtual reality (VR) applications. 
This can allow users to experience VR environments that are highly realistic and immersive.

Augmented reality: NeRF can be used to generate 3D models of real-world scenes that can be used in augmented reality (AR) applications. 
This can allow users to see virtual objects and information overlaid on the real world in a way that is highly realistic and seamless.

3D printing: NeRF can be used to generate detailed 3D models of real-world objects, which can then be used to create physical copies of those objects using 3D printing technology.

Robotics: NeRF can be used to generate 3D models of real-world scenes that can be used in robotics applications. 
This can allow robots to better understand and navigate their surroundings, and to interact with objects in the real world.

These are just a few examples of the potential use cases for NeRF. It has the potential to be applied in a wide range of fields and industries, and it is likely that new use cases will continue to be discovered as the technology develops.


