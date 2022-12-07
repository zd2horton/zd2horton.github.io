---
layout: post
title: Gameplay Programming, Switches and Doors
date: 2019-02-19
excerpt: A task involving the avatar beginning a cutscene in order to open a door.
GPPproject: true
GPPpost: true
tags: [GPP, GPPproject, GPPpost]
category: post
published: true
comments: true
---

This assignment asks for a door to be opened via a switch, transitioning into a cutscene in which pressing the switch unlocks the door.

The initiation takes place via the player entering a trigger space just before the switch, and checking to see through an OnTriggerStay command if they are punching. If they are, it then disables the main camera and changes to the cutscene camera to capture the hit and proceeds to the door to watch the bars move away. The door then opens afterwards and the camera moves back to the player, ending the cutscene.

This task allowed for a broader imagination than the others especially on how the door could open, leading to the barred door. There are some improvements that can be made, including allowing the player to hit from more angles rather than always hitting the button from the front. There is also a strange camera conversion problem which can be seen for a few frames during the camera change back after the cutscene, which in the final "industry" version of the project must be fixed.

[https://www.youtube.com/watch?v=Ihj70n6yMRQ](https://www.youtube.com/watch?v=Ihj70n6yMRQ)

The switch and door:
<a href="https://i.imgur.com/59FhqJe.png"><img src="https://i.imgur.com/59FhqJe.png"></a>

The avatar initiating the cutscene by punching the switch:
<a href="https://i.imgur.com/v28XIPg.png"><img src="https://i.imgur.com/v28XIPg.png"></a>

The door beginning to unlock:
<a href="https://i.imgur.com/8Tf2FJ5.png"><img src="https://i.imgur.com/8Tf2FJ5.png"></a>

The door fully unlocking:
<a href="https://i.imgur.com/ZbZ69WP.png"><img src="https://i.imgur.com/ZbZ69WP.png"></a>