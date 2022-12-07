---
layout: post
title: Gameplay Programming, Group Project Door and Cutscene Mechanisms
date: 2019-04-09
excerpt: Implementation of doors and cutscene cameras in Level 3.
GPPproject: true
GPPpost: true
tags: [GPP, GPPproject, GPPpost]
category: post
published: true
comments: true
---
At the beginning of the level, the player must press the switch to the side. From here the character controller is disabled so that the player cannot move during the cutscene, and the POV switches over to a new cutscene camera which moves over to a designated cutscene point just outside the door. From here the door slides up out of view, disabling the mesh renderer and collider so that it is completely invisible. This then lets the camera move back to the player position, switching to the main camera and enabling the character controller once more and letting them move. An enumerator is then called giving the player a 13 second time limit to go into the room, then switching to another camera which shows the door slide down to its original position after regaining its collider and renderer. This then resets required variables in the trigger script so that if a player fails, they are able to press the switch again.

In the next room after defeating all slimes, the door slides up in a similar way, letting the player cross. With the next cutscene, a new camera shows the door in front of the Simon Says puzzle, starting a coroutine which one by one turns the "lights" above the door into the respective colours required of the puzzle before giving control back to the player.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=wWEd0yJKpSQ" target="_blank"><img src="http://img.youtube.com/vi/wWEd0yJKpSQ/0.jpg" alt="Group Project Door and Cutscene Mechanisms" width="240" height="180" border="10" /></a>

The start of the beginning door cutscene:
<a href="https://i.imgur.com/oOy1qAI.jpg"><img src="https://i.imgur.com/oOy1qAI.jpg"></a>

The door opening:
<a href="https://i.imgur.com/OCnvaBg.jpg"><img src="https://i.imgur.com/OCnvaBg.jpg"></a>

The main temple door opening after killing the slimes:
<a href="https://i.imgur.com/pwNqHqL.jpg"><img src="https://i.imgur.com/pwNqHqL.jpg"></a>

The Simon Says cutscene:
<a href="https://i.imgur.com/LwsojBv.jpg"><img src="https://i.imgur.com/LwsojBv.jpg"></a>

The final door opening after solving Simon Says:
<a href="https://i.imgur.com/4OX9SWM.png"><img src="https://i.imgur.com/4OX9SWM.png"></a>
