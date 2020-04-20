---
layout: post
title: Audio Visual Production, OTVR Update 17
date: 2020-04-16
excerpt: Continued and near finished work on the Bandit Scene.
tags: [AVP, post, AVPpost]
AVPpost: true
category: post
published: true
comments: true
---
The strange silence at end of audio clip issue has been mostly fixed thanks to the conversion of mp3 clips into wav and small tweaks. To add to this, a slightly faster version of the snow audio will now play when the wagon speeds up. This was done in Audacity and not Unity due to Unity's lack of a simple clip speed feature. With this, horse whinnies for the same situation are now in and working fine, and are picked randomly. The script initally failed as it would play multiple whinnies all at once before playing a lone one seconds later, but a small workaround fixed this issue and makes sure the code does not choose a random clip every single frame and attempt to play it. 

From this point on, the highest priority issues are the crashing wagon audio clip in order to finish this scene's clips, the ability to stop the travelling clips in the bandit and town scenes, and work on the repair scene.