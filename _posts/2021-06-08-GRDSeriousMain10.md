---
layout: post
title: Games Research and Development - Bio-Rover Update 8
date: 2021-06-08
excerpt: Documenting the beginnings of light influence.
tags: [GRD, post, GRDpost]
GRDpost: true
category: post
published: true
comments: true
---
A WIP system for influencing the Rover via light has been implemented, using a LightSource tag and an array of potential sources which contribute to influencing the Rover's movement. These sources are in turn checked for legitimacy, and a MoveTowards is used to move the Rover away from it at a consistent speed. In the provided video, another Rover is used as a stand-in "light source" which the player Rover can be influenced from. Currently, the implementation is not too functional as it contradicts the previous torque for the Rover, but this should be ironed out fairly soon.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=VHCSV1uGtqA" target="_blank"><img src="http://img.youtube.com/vi/VHCSV1uGtqA/0.jpg" alt="Light Influence Progress" width="240" height="180" border="10" /></a>