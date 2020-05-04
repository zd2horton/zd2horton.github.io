---
layout: post
title: Audio Visual Production, OTVR Update 16
date: 2020-04-09
excerpt: Miscellaneous fixes and changes.
tags: [AVP, post, AVPpost]
AVPpost: true
category: post
published: true
comments: true
---
The PlayerWagon prefab has now been updated making it easier to use in scenes. This includes the collider used on the top left wheel to detect terrain types, the stage audio script and the WagonAudio prefab containing each terrain clip. A check for wagon speed has also been added for the Bandit Scene in the case of an intense snow wagon audio clip, and a universal check has been completely added so audio stops if the Player Nav Mesh is stopped. However, only the River scene seems to stop the Nav Mesh, as the Bandit and Town scenes do not. Things may need to be altered in order to bring consistency, or another way entirely may need to be used.

Progress Video:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=iSr9bz5v-9E" target="_blank"><img src="http://img.youtube.com/vi/iSr9bz5v-9E/0.jpg" alt="Update 16" width="240" height="180" border="10" /></a>