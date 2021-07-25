---
layout: post
title: Commercial Games Studio - Apex Drive Update 19, Potion Panic Update 1
date: 2021-07-07
excerpt: Building upon the victory animation, and looking into Potion Panic's systems.
tags: [CGS, post, CGSpost]
CGSpost: true
category: post
published: true
comments: true
---
Since PositionUpdate, a script that many aspects such as elimination and the UI scripts depended on to acquire information about the vehicles has become redundant, various scripts have been modified to instead use GameManager (variables such as vehicleManager.raceCars.count being changed to GameManager.Instance.PlayerCount and GameManager.Instance.ConnectedPlayers[i]). As well as this, other factors that were introduced in PositionUpdate like the offscreen timer and eliminated variables have been relocated into the and updated for use in the Player class due to their natures, now utilising getters and setters in order to fit in. As another knock-on effect, the victory animation script has now been able to be fleshed out more easily and now fully uses the winning car's variables in order to dictate what colour Tuk is to be used as well as the number of stars to be displayed. 

With this however, a number of scripts have also been removed or made redundant due to being linked to PositionUpdate or generally being improved on in a different area. This includes the PositionUpdate based variables in RaceManager and EliminationScript, ResetTrackScript, and despite the successful updating of the system, the text placements in BoostBarScript (as discussion has concluded that it may not be required in an elimination based local party game, as positions will only be used to determine where the camera should follow). 

As of now, the systems have been tested through instantiating vehicles by hand through RaceManager, which has necessitated the initial untoggling of EliminationScript due to it presuming a solo player has won during the instantiating of vehicles. Once the other method is used, these issues can be reversed and thus this alongside the appropriate modifications to have the animation fit with the game's atmosphere more will be highest priority.

Currently, the beginnings of Potion Panic are emerging with looking into its current systems, and starting contributions in specified areas. A large focus will be placed on this over the next week, and developments should sprout more with further understanding of the overall project. 

<a href="http://www.youtube.com/watch?feature=player_embedded&v=Siu4rrGxo7o" target="_blank"><img src="http://img.youtube.com/vi/Siu4rrGxo7o/0.jpg" alt="Round Animation and Learning Systems" width="240" height="180" border="10" /></a>