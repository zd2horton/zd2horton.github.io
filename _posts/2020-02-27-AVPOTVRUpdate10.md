---
layout: post
title: Audio Visual Production, OTVR Update 10
date: 2020-02-27
excerpt: Fully implementing audio and fixing the issues.
tags: [AVP, post, AVPpost]
AVPpost: true
category: post
published: true
comments: true
---
Overall, the wagon audio system now functions without issue. With before, the audio would change based on trigger areas that the wagon would enter, large in size in order to compensate for the viewing port of the wagon. This caused many issues, one of which possibly being the issues from the wooden sounds. As well as this, the audio being implemented in this manner also made for inconsistent results. The script in the new method now uses OnCollisionEnter over OnTriggerStay, as collisions take place on a slightly outstretched box collider positioned on a front wheel rather than through using tagged trigger areas (with road sections tagged instead). This now gives fully consistent transitions to different terrain audio, and alongside the script using a loop to compare the terrain collided with and wagon audio names the system can now be used on a universal scenario rather than just the current one. From here, the existent audio can be improved and scenario 2 can be worked on.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=p0ScqdL_Rao" target="_blank"><img src="http://img.youtube.com/vi/p0ScqdL_Rao/0.jpg" alt="Update 10" width="240" height="180" border="10" /></a>