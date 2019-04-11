---
layout: post
title: Gameplay Programming, Moving Platform Sequence
date: 2018-03-18
excerpt: Implementing various types of platforms.
GPPproject: true
tags: [GPP, GPPproject]
category: post
published: true
comments: true
---
This assignment involves making platforming sequencing allowing floating or submerged platforms, and mechanical platforms as well as possibly dipping when the player steps on it. 

My implementation has platforms moving on splines, the first moving on two different curves as it changes between the two when finished with the previous. It is also dependent on the player landing on it, as doing so turns a variable in the platform's path movement script allowing movement true and parenting the avatar to itself. As well as this, a second platform is completely independent of the player, appearing at the beginning of the spline once finished. This in turn with the start and end points of the spline and the cover they have gives the illusion that another platform is appearing from the left side once the previous disappears on the right.

While the platforms work well, more mechanical platforms should have been made, which could be done by having a platform move before stopping after a certain amount of time, and then moving again. This was not a method that I did consider, as I believed the implementation to be more complex. This is also a similar case with reactive platforms, which could go down a little upon being weighed down and return once left.

[https://www.youtube.com/watch?v=NUye-eo-S60](https://www.youtube.com/watch?v=NUye-eo-S60)

The player dependent platform:
<a href="https://i.imgur.com/DpVoBAQ.jpg"><img src="https://i.imgur.com/DpVoBAQ.jpg"></a>
<a href="https://i.imgur.com/HsPQk6L.jpg"><img src="https://i.imgur.com/HsPQk6L.jpg"></a>


The independent moving platform:
<a href="https://i.imgur.com/OAxkNKl.jpg"><img src="https://i.imgur.com/OAxkNKl.jpg"></a>
<a href="https://i.imgur.com/ehgeXzL.jpg"><img src="https://i.imgur.com/ehgeXzL.jpg"></a>