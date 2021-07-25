---
layout: post
title: Commercial Games Studio - Apex Drive Update 20
date: 2021-07-14
excerpt: Refining the UI and victory animation further.
tags: [CGS, post, CGSpost]
CGSpost: true
category: post
published: true
comments: true
---
As of current, the banner has now been changed to use a gradient from the game logo's red and orange in order to fit the game's mood more appropriately and clash a little better with the vehicles, while the stars have been blackened and shrunk to fit into both the banner's style and measurements. As well as this, the previous boost bars have now been replaced with the lobby scene's player icons, which consequently required an overhaul of the boost bars script. This included the outright removal of the slider and image variables (as the slider and image functions are now fulfilled by the icons' borders, being able to handle the diminishing through the fill amount as well as the red to yellow gradient implementation) and general optimisation of the code (filtering repeated loop declarations to one overall instance).

When testing this implementation, the borders' colours and the victory banner clashed extremely heavily even when changing the colours of the borders, resulting in the decision to show only the victory animation when it is active. This was initially attempted through the creation of a new "winner" player variable toggled in EliminationScript and checked in BoostBars in turn giving a switch for when to set the player icons to be inactive, but this did not go as planned due to this variable being made false immediately after being set to true. Thus, a more direct method of setting inactivity was implemented in the RoundVictoryAnimation as such a UI element would have an easier time both accessing the icons and providing the neccessary timing for the procedure. Once this was implemented, the victory animation's transition seconds were all then nullified as to rectify the animation running past the 3.5 seconds given to it and overlapping with the player icons as a result.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=p89ijJqDjWQ" target="_blank"><img src="http://img.youtube.com/vi/p89ijJqDjWQ/0.jpg" alt="UI Updates" width="240" height="180" border="10" /></a>