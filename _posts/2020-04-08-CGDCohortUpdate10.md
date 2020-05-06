---
layout: post
title: Commercial Games Development - Cohort Jam Update 10
date: 2020-04-08
excerpt: Implementation of audio events for the vending machine.
tags: [CGD, post, CGDpost]
CGDpost: true
category: post
published: true
comments: true
--- 
As of now, the audio team have supplied audio for when the vending machines fall over, crush a pawn or shake. The falling and crushing audio events have been implemented without issue as they are oneshot (requiring a simple PlayAudioOneShot command), however the shaking audio still needs to be placed in appropriately as it is a looping clip. Due to this, a differing way will need to be found for this audio to play.

Video:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=TjzC7Cn-AD4" target="_blank"><img src="http://img.youtube.com/vi/TjzC7Cn-AD4/0.jpg" alt="Cohort Update 10" width="240" height="180" border="10" /></a>