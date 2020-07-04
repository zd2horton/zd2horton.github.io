---
layout: post
title: Commercial Games Development - Sound Jam, Update 2
date: 2019-12-02
excerpt: Progress with the character and its animations in the Sound Game Jam.
tags: [CGD, post, CGDpost]
CGDpost: true
category: post
published: true
comments: true
---
As of now, the animations for the avatar have now been fully implemented and are working as intended. If the player movement code detects that the player is not moving their character, the idle animation will play while either a walking or running animation (depending on use of the shift key, also doubles speed) will play, when detecting a movement key press. Jumping was the hardest to implement, as in various attempts to have it properly work either the jump animation or the walking and idle animations would be sacrificed in return for the other. However, this was able to be overcome when the jumping bool for the animator was replaced with a trigger, and the jumping animation given exit time. As a result of this, the jumping animation will be set off by a trigger that is turned on whenever the space key is pressed and a jump is recorded, playing through the entire animation before the player hits the ground and returns to idle. 

A "capturing" animation was also implemented, this being through a mask. Initially after setting the mask up on its own layer and implementing it through the code, the body moved all at once which was contradictary to the map set up before in which it ignored the lower half of the body. The root of this was eventually found to be a custom set of options in the transform part of the mask, where the appropriate options had to be chosen in order to get the mask functioning properly. From here, a weapon or capturer will need to be placed into the avatar's hands for the animation, and various juice will need to be implemented in likeness.

The problematic animations that were fixed:
<a href="https://i.imgur.com/eJIqHSb.gif"><img src="https://i.imgur.com/eJIqHSb.gif"></a>
