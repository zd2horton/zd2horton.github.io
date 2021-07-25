---
layout: post
title: Commercial Games Studio - Apex Drive Update 13
date: 2021-06-05
excerpt: Further UI implementation through text.
tags: [CGS, post, CGSpost]
CGSpost: true
category: post
published: true
comments: true
---
Implementations of a ranking system are underway in order to assist with the UI bar text. Currently, this is done through looping through each vehicle and comparing collider hit and lap count amounts to the others in the game. As the colliders signify checkpoints on the track, hitting more would on average result in the superior player being placed in front of the others and thus this increments an "aheadOf" variable which keeps track of how many vehicles the current is ahead of. Once this number is attained, it is then found which position it corresponds to in relation to how many vehicles are on thr track. Initially, a switch case was intended for this but was removed due to the syntax not being able to use non static values, and an intended enumerator was also removed due to being made redundant through the aforementioned implemented comparison method. As of current however, an issue has been realised which causes only the top left text to read 1st even if Player 1 is not leading, as well as the consumption of the other players' bars by unintended players in some cases. This is likely due to the RaceManager swapping the positions of the vehicle array, but more information will be found through investigation.