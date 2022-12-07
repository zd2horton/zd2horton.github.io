---
layout: post
title: Gameplay Programming, Collectables
date: 2019-02-19
excerpt: The second task in Unity for Gameplay Programming involving collectables.
GPPproject: true
GPPpost: true
tags: [GPP, GPPproject, GPPpost]
category: post
published: true
comments: true
---

The task requires the implementation of two power ups, one for a double jump and one for a temporary speed boost, both of which including particle effects. 

In order to progress any further with the overarching assignment, I have fixed the avatar's movement to make it fully comply with the player's input. This uses the same code from before but is written in a more polished fashion. Jumping is now also implemented fully, and the temporary camera has been atuned further to observe the avatar's actions. 

The power ups implemented work as intended and leave particle effects behind when picked up, with the double jump giving the player another jump if they press space during the descent of their first jump and the speed boost power up giving the player a 4 second boost in speed when holding shift. The effects are also able to stack, giving the player an elongated jump when running with the speed boost. 

There is notable room for improvement, most notably select animations transitioning to any aerial movement. When normally moving around, the avatar jumps properly however when the avatar lands, they will move around in the idle animation for a number of seconds as if stuck in exit time, after which animations will begin to function normally again. As well as this, the flip animation used for the double jump seems to not function and instead has the avatar squat during and before an idle animation which will be applied until landing. Both of these problems seem fixable by tinkering with animation booleans in the animator and inside of the code. To add, other alterations could include adding particle trails for the speed boost and particle effects onto the items themselves while they are in the world.

[https://www.youtube.com/watch?v=k5QpSrsSK-s](https://www.youtube.com/watch?v=k5QpSrsSK-s)

The avatar approaching the double jump power up:
<a href="https://i.imgur.com/ej5kUd7.png"><img src="https://i.imgur.com/ej5kUd7.png"></a>

The avatar jumping successfully (left) and the avatar jumping instantly after landing(right):
<a href="https://i.imgur.com/9xZ40Xr.png"><img src="https://i.imgur.com/9xZ40Xr.png"></a>

Collecting the double jump, which explodes into a flurry of red petals:
<a href="https://i.imgur.com/CRpZVyG.png"><img src="https://i.imgur.com/CRpZVyG.png"></a>

Collecting the speed boost, which erupts into a pillar of fire:
<a href="https://i.imgur.com/kOxu1I1.png"><img src="https://i.imgur.com/kOxu1I1.png"></a>