---
layout: post
title: Gameplay Programming, 2.5D Spline Gameplay
date: 2018-03-11
excerpt: Gameplay following a 2.5D segment using Bezier curves.
GPPproject: true
tags: [GPP, GPPproject]
category: post
published: true
comments: true
---
This task requires the implementation of spline segments in a level, overriding controls and camera properties for these 2.5D segments.

The system implemented first allows for creation of a Bezier curve, using 4 nodes in the calculation which can be repositioned anywhere, in turn affecting the output curve in the editor. Once the player or other applicable object touches the beginning node in gameplay, they are placed into the curve and while inside their movement either decreases or increases the "t" value in the Bezier curve equation, in turn placing the resulting value as the object position. Once the "t" value has reached 1, the player is placed onto the path to the next node in the sequence or is taken off the curve if they have reached the end by disabling the script.

The biggest problem with this implementation is that the player does not rotate accordingly with the path, neither do they turn around if walking backwards in the spline. This may be due to the curve fixing the object's rotation, not letting it rotate in any other way. As well as this, walking backwards even beyond the start keeps the player fixated inside, even though there is no spline path present. A similar issue is the inability to go back through the spline via the end. This is problematic and needs fixing, as players may need to backtrack through a spline area.


[https://www.youtube.com/watch?v=gyoM1d2A9EE](https://www.youtube.com/watch?v=gyoM1d2A9EE)

The beginning of the spline:
<a href="https://i.imgur.com/Uj1kjHt.jpg"><img src="https://i.imgur.com/Uj1kjHt.jpg"></a>

The issue of the inability to turn in the spline:
<a href="https://i.imgur.com/mfj6Dr9.jpg"><img src="https://i.imgur.com/mfj6Dr9.jpg"></a>


Walking backwards in the spline, causing the player to still be stuck as well as the inability to go through the tail end:
<a href="https://i.imgur.com/kGQGrRR.jpg"><img src="https://i.imgur.com/kGQGrRR.jpg"></a>
<a href="https://i.imgur.com/wgsXsYa.jpg"><img src="https://i.imgur.com/wgsXsYa.jpg"></a>