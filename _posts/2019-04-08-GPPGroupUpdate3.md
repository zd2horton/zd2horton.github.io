---
layout: post
title: Gameplay Programming, Group Project Update 3
date: 2019-04-08
excerpt: Fixing previous issues, and adding the patterned platform segment.
GPPpost: true
tags: [GPP, GPPpost]
category: post
published: true
comments: true
---
The previous error showcased with the switch has been fixed, allowing for the player to open the door again if they failed the previous time. This was caused through a boolean not staying true for long enough, meaning that the required state was not shared with other scripts. The patterned platforming section, or in simpler terms Simon Says, has been implemented at a basic level. All of the platforms involved are children of an empty gameobject, and if stepped on send a flag to their parent's script telling it they were collided with. This uses "getSiblingIndex", meaning that as a result the gameobject is able to use said index to access the child affected and thus its tag, reading in the colour tag and applying a score onto the tile being stepped on. This then checks against a list of correctly ordered combination of button hits for the Simon Says and decides if the step was incorrect. If so, it wipes progress and restarts. 

For the next update, I would like to implement "win" and "lose" conditions for the puzzle, the win condition opening the door in front of the puzzle and the losing condition fading the screen before placing the player back before the puzzle and deducting some health. I would also like to fix reactivity for the platforms the player can step on, as this was implemented but does not seem to be working.


<a href="http://www.youtube.com/watch?feature=player_embedded&v=xiG28q_9-nQ" target="_blank"><img src="http://img.youtube.com/vi/xiG28q_9-nQ/0.jpg" alt="Group Project Update 3" width="240" height="180" border="10" /></a>

A cutscene showing the player the Simon Says order:
<a href="https://i.imgur.com/KbsG81c.jpg"><img src="https://i.imgur.com/KbsG81c.jpg"></a>

The player playing the Simon Says puzzle:
<a href="https://i.imgur.com/VvO1m7d.jpg"><img src="https://i.imgur.com/VvO1m7d.jpg"></a>