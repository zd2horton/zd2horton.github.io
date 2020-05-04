---
layout: post
title: Audio Visual Production, OTVR Update 9
date: 2020-02-20
excerpt: Progress on the code for terrain audio.
tags: [AVP, post, AVPpost]
AVPpost: true
category: post
published: true
comments: true
---
After a lot of toying around, it seems that the scenario finally swaps the audio out when required. This was done through vastly expanding the hit box as well as using OnTriggerStay instead of Collisions, and as well as this the function was altered so that there is one If situation to process rather than a handful. However, when viewing the scene through a certain angle the wooden sound effects become distorted, and currently the cause is uncertain. More investigation will need to be done in order to find the solution to this. 

<a href="https://i.imgur.com/KOdaGzL.png"><img src="https://i.imgur.com/KOdaGzL.png"></a>