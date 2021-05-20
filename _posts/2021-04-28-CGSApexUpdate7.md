---
layout: post
title: Commercial Games Studio - Apex Drive Update 7
date: 2021-04-28
excerpt: Creating a concrete elimination system.
tags: [CGS, post, CGSpost]
CGSpost: true
category: post
published: true
comments: true
---
Using newly placed eliminated and winner booleans in PositionUpdate, the elimination script is now able to detect a winner. This is done through the initialisation of a total eliminated variable in update, incrementing when a successful elimination or elimination check is performed for a vehicle and finally causing the winner boolean to become true for that specific vehicle once the total eliminated is equal to the number of vehicles minus one. If the number of eliminated vehicles is equal to the total minus 1, the remaining car is given the winner.

As well as this, progress is being made on Name Tags for players. Many attempts and consequences have been observed, such as vehicles transforming into TextMeshPro objects when the component is added to them directly to the prohibited addition of multiple TextMeshPro components into the canvas to eventually, individual empty GameObjects that are created and placed into the canvas as children. This latter technique bore more desirable results, in turn being able to hold the TextMeshPro components and add the vehicle's name to itself. Efforts are being made to visualise the tags properly as at the moment, the text objects are placed further away despite being converted to the screenpoint.