---
layout: post
title: Commercial Games Studio - Apex Drive Update 5
date: 2021-04-09
excerpt: Progress with the elimination system.
tags: [CGS, post, CGSpost]
CGSpost: true
category: post
published: true
comments: true
---
As of current, implementation on the elimination system is progressing well. Once integrated into the game's newly created camera system, the method of elimination involving boundaries was found to work. At first, the method of a list finding the players through tags was used, but this was not optimal and did not link in any way to existing scripts. Once the project was explored the pre-existing list was replaced with the usage of the race manager, in turn giving direct access to the players and also gave the same finishing result. In order to test the system, the first vehicle to exit the view was immediately eliminated and though this proved the system to be functional it was not suitable for the game as players who boost ahead may be eliminated unfairly. Thus, a timer was set out to be implemented however the current method of using an ienumerator does not seem to function, assumedly due to issues to do with exiting itself according to breakpoints. This will be looked into and ideally fixed promptly.

As well as this, pitches have made inside the group for the third workstream. The first, a souls-like open world adventure, involves the use of a spear headed rope weapon in combat in such ways as pulling enemies to be closer, lassoing them or tripping them. The second pitch, Potion Panic, a competitive party game, involves the acquiring of ingredients to make spells for use against other players with gamemodes possibly including timed or survival matches, stage hazards possibly being a feature. The final game, Cloak, is a co-op stealth game making use of both PC and mobile players. The theme, being in deep space travel, follows the potential presciences of supernatural or alien forces with the computer player completing tasks while avoiding said prescience. Alongside this, the mobile players assist the computer player through hacking based minigames and guiding them with an available map. As for the prescience, it will be able to disable the mobile players at points and hide from the computer player. Overall, the ideas are notably strong however for both implementation and gameplay, Cloak feels the most appealing. This is due to the co-operation of players, replayability and the communication between the computer and mobile applications.