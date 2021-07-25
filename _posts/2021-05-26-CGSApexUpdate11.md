---
layout: post
title: Commercial Games Studio - Apex Drive Update 11
date: 2021-05-26
excerpt: An in person demo, and general modifications.
tags: [CGS, post, CGSpost]
CGSpost: true
category: post
published: true
comments: true
---
In terms of overall progress, various systems have been fixed. Some issues were confronted in other branches over the winner state not being reached, with the root cause quickly being found to be the eliminatedTotal variable. A check was added for previously eliminated vehicles to add to it in the case of a new loop, with it resetting to 0 each new loop. However, with a circumstance such as Player 2 being eliminated, the total would reset to 0 due to the loop ending and thus once Player 1 would be processed the if statement used to find the winner would not be made true as the eliminatedTotal would be too low. Thus, eliminatedTotal has been made a global variable and the refresh satisfaction check has been removed, which has remedied the problem. As well as this, the Vehicle Colour script has been made to run after every other script as otherwise it seems to not function due to Unity choosing to run it before other scripts it depends on for information and data.

The in person demo for the game mostly proved to be functional, however when confronted with four input controllers the game only allowed two. Despite these issues and a small handful of others pertaining to others' systems, both their systems and the systems explained in detail in these entries functioned as they were intended to. 

For Cloak's progress, a meeting was called to discuss the viability of continuing with a game with such scope despite there being such little time to bring three games to alpha, two to beta and one to gold. It was eventually decided upon that the idea would need to be dropped, in turn revitalising the Potion Panic idea from before while maintaining a notable amount of art direction from Cloak itself. Due to the showcased progress on both the AltSpaceVR and Apex Drive assignments in the transpired time window, this seems to be the optimal decision as otherwise Cloak may have not been given the attention it required, taken too much attention from the other two tasks or may have perhaps even been unsuccessful for developing. With this, preparations and designs for Potion Panic will begin, with level and minigame designs being some of the first required for the foundation of the game's development.