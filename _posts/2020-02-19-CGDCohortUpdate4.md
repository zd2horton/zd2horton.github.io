---
layout: post
title: Commercial Games Development - Cohort Jam Update 4
date: 2020-02-19
excerpt: Clarity given for elements related to the vending machine.
tags: [CGD, post, CGDpost]
CGDpost: true
category: post
published: true
comments: true
--- 
This week, information has been gained that can help the continuation of planning out the event's programming. As well as small pieces of advice for such things as interacting with the pawns, clarity on the event manager has been given alongside information on what the level design team require out of the event (such as how it can be rotated in the level editor, and the possibility of them not being against a wall at all times). The event manager uses prefabs and loops through all tiles in a new level to get events and store them, placing a timer until the event occurs at which it instantiates. Due to this, the vending machine will need to work around this limitation as it will be created at the start of the map, meaning that the manager would instead be used for activation of the event (in where it wobbles). This could also call for a hard-coded solution in which a function for turning the machines on is made, and when the events are deactivated, they use an ID to call to the eventmanager in a CheckIfActive function.

The way in which the Event Manager initialises events:
<a href="https://i.imgur.com/mOOZPKw.png"><img src="https://i.imgur.com/mOOZPKw.png"></a>