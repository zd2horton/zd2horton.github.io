---
layout: post
title: Commercial Games Development - Cohort Jam Update 7
date: 2020-03-11
excerpt: Altering the code to work with the tile system and other points.
tags: [CGD, post, CGDpost]
CGDpost: true
category: post
published: true
comments: true
--- 
The event has now been coded to fit the mould of the tile system. Originally, it was thought that this was not an implementation that required exterior help but done through such as it needed to be registered as a tile type. Through this, the event uses the tiles at positions it needs to analyse (for instance, the position of the machine now uses GetTileAtPosition of itself) and will only set the pre requisite to fall if the tile it decides to fall on is not a wall. As well as this, a different prefab has been made for a fallen machine as previously discussed and handles the code for killing pawns instead of the base script. This instantiates alongside the existing machine and acts as the blockade part of the machine. While the exact documentation is somewhat messy looking on first glance, effort will be made in understanding it as much as possible in order to fully contribute to the vending machine event.

<a href="https://i.imgur.com/lAekMTH.gif"><img src="https://i.imgur.com/lAekMTH.gif"></a>