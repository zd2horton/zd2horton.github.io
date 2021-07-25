---
layout: post
title: Commercial Games Studio - Apex Drive Update 17
date: 2021-06-23
excerpt: Fleshing out and development of the elimination system.
tags: [CGS, post, CGSpost]
CGSpost: true
category: post
published: true
comments: true
---
Currently, the elimination system is being fleshed out in order to link more appropriately with the game classes as well as creating a victory animation once each round is over. Each round and game winner is passed through an instance of the GameManager as it holds all relevant instance dependant information, with the correct player being allocated via linking the CarModule PlayerID. This value was somewhat difficult to obtain at first, as many unsuccessful methods were thought of such as using the CarInputHandler's currentPlayer. As of current, the implementation has been done through attaching Core Car Module to the "Auto Rickshaw" component of each vehicle and altering appropriately so that the player IDs are correct. At first, tests done without breakpoints would add two round wins per win, seemingly due to the code eliminating the eliminated player(s) again and thus fulfilling the gate quota of the system giving another victory. This was fixed via a "processed winner" variable that closes off the elimination process once a winner has been processed, and as the script is currently reset each new game due to scene switching, this allows for an automatic toggle which helps restrain proceedings. From here, the animation will be worked on.

Click the video to view today's update:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=Cx18XzPYsYs" target="_blank"><img src="http://img.youtube.com/vi/Cx18XzPYsYs/0.jpg" alt="Elimination System Further Development" width="240" height="180" border="10" /></a>