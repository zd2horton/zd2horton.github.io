---
layout: post
title: Games Research and Development - Bio-Rover Update 4
date: 2021-05-18
excerpt: Current progress in documentation and the project.
tags: [GRD, post, GRDpost]
GRDpost: true
category: post
published: true
comments: true
---
The Game Design Document has currently been updated to include an overview of various aspects about the project, from the design decisions guiding the game to the Bio-Rover's own physical capabilities and potential gameplay loops. With just smaller categories missing such as pre-existing examples to research and what to consider for future development, the document will undoubtedly act as an essential guide to the project's development, as well as a major reflective piece that can be evaluated once current development ceases. 

To add, a Bio-Rover model has been crafted from an external source and is able to be used in the project, with some shader issues requiring that the model be used as not one mesh but a collection of them. Once shaded correctly, progress began on initial movement and with this, Rover rotation to give a more natural sense of flow and animation. This was done through the adding of torque to the Rover's RigidBody as the player influences it, with a small issue of the Rover falling through terrain being fixed through adding a Sphere Collider. As such, basic movement is now possible for the Rover however the next steps would be to further integrate basic gameplay elements, before building upon this with such things as light source influence.