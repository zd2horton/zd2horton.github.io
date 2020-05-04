---
layout: post
title: Audio Visual Production, OTVR Update 18
date: 2020-04-28
excerpt: Mostly finished, apart from potential small changes.
tags: [AVP, post, AVPpost]
AVPpost: true
category: post
published: true
comments: true
---
In all, many issues have now been fixed and audio is almost entirely finished. The wagon viewbox's controller uses the distance between the player and current destination to determine whether the wagon is moving or not, and the resulting variable is now used to effectively end and start audio for when the wagon stops. While using this method creates a second delay or so before audio begins playing again, it has helped solve a longtime issue that would otherwise be more noticeable.

In terms of other fixes, most audio clips have been altered similarly to previous clips to fit with looping better. This was initially done in order to get rid of a notable gap when the trading scene's crowd ambience looped, and was applied to the rest of the looping clips in case of a potential issue similar to the one that needed fixing. 

After finally editing a wagon crashing clip together, it became apparent that it was not required at the end of the bandit scene and thus has gone unused. The repair scene has now had work fully complete on it, with an ambience piece incorporating the usable sections of the ZOOM audio acquired previously. The scene also makes use of various working clips for the hammer, nail and iron stores in a similar fashion to the tinkering audio in the trading scene, and the wagon's terrain audio in this scene is an altered version of the river scene's road audio layered with rickety wheel audio for a shaky travel feeling up until the wagon is fixed.

A notable issue with the iron store audio in particular was that it at various times like with certain town trading pieces were audible either too early or immediately. This was eventually fixed by shrinking the size of the overall component down as well as the volumetric radius and range so that it would only be audible near the area where the wagon stops.  

With the wagon terrain audio, the initial audio with the faulty wheel is used first, before being changed using a new function in StageAudio which uses the viewbox's "RepairController" once it recognises all items have been purchased. This then gives the signal that the wagon can move on, and the clip is changed to the unaltered road terrain audio from the river scene which will be audible once the wagon begins moving.

For additional improvements, if there is time then spacing for audio could be further optimised to improve the experience, while potential music for scenes and additional audio can be used to flesh scenes out. This would include such examples as audio for the jack store in the repair scene (which does not yet have audio due to lack of ideas on possible audio), and indicative audio which would help confuse players less at points of decision. 

<a href="https://i.imgur.com/LUIgqCD.png"><img src="https://i.imgur.com/LUIgqCD.png"></a>

<a href="https://i.imgur.com/2hNF46N.png"><img src="https://i.imgur.com/2hNF46N.png"></a>

Progress Video:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=5hFChl3QSHo" target="_blank"><img src="http://img.youtube.com/vi/5hFChl3QSHo/0.jpg" alt="Update 18" width="240" height="180" border="10" /></a>