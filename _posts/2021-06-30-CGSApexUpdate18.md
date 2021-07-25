---
layout: post
title: Commercial Games Studio - Apex Drive Update 18
date: 2021-06-30
excerpt: Creating the initial victory animation.
tags: [CGS, post, CGSpost]
CGSpost: true
category: post
published: true
comments: true
---
As of current, the base victory animation has been implemented. The initial idea involved the flowing in of a banner alongside the winning vehicle driving in with an angle, followed by their round wins represented by stars. Attempts were made to replicate this, firstly with visualising the models in the Canvas space. These proved to be unfortunately fruitless however, and it was eventually found that such a thing would not work in HDPR mostly due to its emphasis on the usage of one camera per scene. 

Thus, 2D sprites have been created for the implementation and will sweep across the banner unveiling the round wins for that player. The UIBarCanvas prefab has been updated to include the elements to be used, and animations have been created for the appropriate elements. Finally, an animation script has been created to implement this logic (using an IEnumerator which toggles the Animator booleans to create the animation), and various others have been modified to better suit the circumstances (ResetTrack will be used to call the animation functions). The animation currently functions with default settings, and implementation from here will use the other systems to determine settings once in the game.

Click the video to view today's update:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=EhD2S06pbsc" target="_blank"><img src="http://img.youtube.com/vi/EhD2S06pbsc/0.jpg" alt="Victory Animation Progress" width="240" height="180" border="10" /></a>