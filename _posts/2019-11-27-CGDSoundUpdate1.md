---
layout: post
title: Commercial Games Development - Sound Jam, Update 1
date: 2019-11-27
excerpt: Current progress and issues with the 3rd Game Jam.
tags: [CGD, post, CGDpost]
CGDpost: true
category: post
published: true
comments: true
---
Initially, an issue arose where an applicable player avatar was not found, but after various searches a sci-fi esque avatar was found. Animations are toggled via the operation of booleans, written into the player movement script so that each animation state can be played when required. However, there is currently a problem in which the Axes for various inputs such as jumping and moving are not being read continuously, meaning that an animation will only play once before not playing again. This will need to be solved in order to progress, as due to the wild nature of the Rigidbody's velocity, a simple check for 0 in a value of the velocity vector cannot be used.