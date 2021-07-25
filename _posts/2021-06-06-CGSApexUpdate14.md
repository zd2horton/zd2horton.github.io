---
layout: post
title: Commercial Games Studio - Apex Drive Update 14
date: 2021-06-06
excerpt: Finding remedies to previous issues, and optimising code.
tags: [CGS, post, CGSpost]
CGSpost: true
category: post
published: true
comments: true
---
The main issue from before in which incorrect player information would be relayed has now been fixed. In this fix lead by a peer in the team, an "original raceCars" list is used which is never updated alongside a GetPosition method which upon being called verifies the vehicles and returns their current position in the array corresponding to the race, which should mean that the raceCars array carries the vehicles in order of ranking. This in turn causes the previous way of determining the positions to be redundant, and the non updating array is used for both setting the sliders and setting the text.

As well as this, it has been decided that a uniform colour bar would fit the project more than a gradient esque bar, so this pursuit has been dropped. To add, a command in Color.Lerp visually performs the same function as the setup and use of a gradient, so this has also been replaced as to be more proficient.