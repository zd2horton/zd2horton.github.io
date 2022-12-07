---
layout: post
title: Gameplay Programming, Basic Avatar Project
date: 2019-01-29
excerpt: Our first Unity task for Gameplay Programming, involving implementing a basic avatar.
GPPproject: true
GPPpost: true
tags: [GPP, GPPproject, GPPpost]
category: post
published: true
comments: true
---
Our overarching assignment for Gameplay Programming is to create a game with gameplay elements close to The Legend of Zelda, and with camera and control schemes close to 3D Super Mario Bros. games such as Super Mario 3D World. This will be accomplished and iterated through many activities, this being the first of such.

This task involves creating a basic Unity avatar which can walk, jump and perform other basic actions. With this, I have created an avatar which is able to move around, using a direction combined with the user given speed in order to set the avatar's velocity. Previous systems attempted to use such aspects such as adding force to the rigidbody itself or affecting the translation of the entire avatar itself, but these either did not work altogether or created undesirable results. 

However, the movement is very slippery and can often go against the player's inputs. Such examples of this include visually walking in reverse to the player's direction (such as walking away from the camera when walking forwards if tampered with enough) and walking in strange diagonal lines that swerve at points when attempting to walk diagonally which also do not comply with the direction the avatar is facing. This must be improved in order for the player to begin playing properly and should be improved with a system that instantly complies with the user's direction and, if needed, can turn without affecting the arc or line at which the avatar walks. 

The turning of the player was more difficult to implement, but was more successful than the movement of the player. This involves using a target rotation and Quaternions to angle the player with the speed, direction they're holding, and delta time in order to rotate the avatar smoothly. Previous implementations of this also included manipulating the transform of the avatar and incorrect manipulation of the rigidbody, both resulting in incredibly incorrect results where the avatar upon moving would rotate around very quickly either on ground or into the air.

While this seems to be fairly functional, it also seems to be a huge catalyst in the movement's problems, as it very clearly seems to be adding to the abnormal angles that the player moves in if they attempt to walk and rotate at the same time.  As a result, further improvements would require for the rotation systems to either not interlock with forward and backward movements, or interlock as to not damage how the avatar moves should they choose to walk while rotating themselves.
 
The camera will also be improved, as it is only currently a basic follow camera with some ability to drag around and view surroundings. The final camera should be similar to Super Mario 3D World in which it is able to follow the player and pivot around somewhat before returning back to position should the player stop manipulating it.

[https://www.youtube.com/watch?v=RBNcEquc4SI](https://www.youtube.com/watch?v=RBNcEquc4SI)

The punching animation implemented:
<a href="https://i.imgur.com/4TLQVUY.png"><img src="https://i.imgur.com/4TLQVUY.png"></a>

The jumping animation implemented, requiring further implementation in order to jump fully:
<a href="https://i.imgur.com/kpoBK2F.png"><img src="https://i.imgur.com/kpoBK2F.png"></a>

The avatar walking forwards but facing backwards, another issue that upon further iteration will be solved:
<a href="https://i.imgur.com/Xn6AEy6.png"><img src="https://i.imgur.com/Xn6AEy6.png"></a>