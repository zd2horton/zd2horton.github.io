---
layout: post
title: Gameplay Programming, Controllable Follow Cam
date: 2019-03-04
excerpt: A follow cam assignment.
GPPproject: true
GPPpost: true
tags: [GPP, GPPproject, GPPpost]
category: post
published: true
comments: true
---
This task required a slick follow cam that the player could control similar to a console game's (for example, a 3D Super Mario game) and locks onto the four directional axes.

The initial camera system is a basic method controlled using the arrow keys, and uses the camera's eulerAngles value to check whether the camera can rotate which is decided by comparing the value with boundaries depending on the rotation direction (for example, the camera can only rotate up 45 degrees due to the boundaries of rotating up being 0 and 45). After checking if the current eulerAngles falls into the required boundary, it uses a RotateAround to rotate the camera around the avatar.

While it allows player control, the implementation is very problematic as it will very often skew the camera in absurd positions, and also tends to lock in the y axis before only unlocking after much effort from the player. This system also requires the camera to be a child of the avatar, which is not an optimal solution.

This was fixed in a newer and more complex implementation, first setting an initial offset distance for the camera to be staged at as well as acquiring the avatar and camera transforms for use. The system then calculates the distance from the player and the offset distance as well as the current distance using this in a Lerp function before allocating this to the camera's position. After this, it calculates similar values for the camera's rotation using Slerp instead of Lerp.

Due to this, the camera now feels more natural, sitting a little behind the player and reacting in proportion to their velocity. This can be seen if the player picks up the speed powerup, which when used causes the camera to pull back as they run and returns to normal speed when the powerup runs out. Rotation is dictated via the player rotating themselves, which does take away from the controllable aspect of the assignment however as a result rotation feels smooth and does not skew like the previous method. To improve this implementation, I will add the ability to rotate upwards as well as rotation using arrow keys independent of player rotation.

[https://www.youtube.com/watch?v=xw2ZNnud0Xk](https://www.youtube.com/watch?v=xw2ZNnud0Xk)

The initial camera system:
<a href="https://i.imgur.com/O2E38gy.jpg"><img src="https://i.imgur.com/O2E38gy.jpg"></a>

Skew and eventual camera lock:
<a href="https://i.imgur.com/0Zi53CN.jpg"><img src="https://i.imgur.com/0Zi53CN.jpg"></a>
<a href="https://i.imgur.com/7wg5Gcq.jpg"><img src="https://i.imgur.com/7wg5Gcq.jpg"></a>

The new camera system, using Lerps and offsetting to provide a higher quality system:
<a href="https://i.imgur.com/utydd51.jpg"><img src="https://i.imgur.com/utydd51.jpg"></a>

The pulling of the camera, shown with the speed powerup:
<a href="https://i.imgur.com/b6Qqo2I.jpg"><img src="https://i.imgur.com/b6Qqo2I.jpg"></a>