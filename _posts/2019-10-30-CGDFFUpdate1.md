---
layout: post
title: Commercial Games Development - Foundary Frenzy, Update 1
date: 2019-10-30
excerpt: An update on my portion of Foundary Frenzy.
tags: [CGD, post, CGDpost]
CGDpost: true
category: post
published: true
comments: true
---
Currently, Foundary Frenzy's Debugger is progressing well. Bugs now spawn from various places outside of the screen and flow in, travelling into the middle and stopping. This is done through using a spawner prefab and script that sets a random time limit, which after being met picks a random side (child) to spawn from, then using the side to generate a random set of co-ordinates for a bug to instantiate from. Initially, there was an issue where the bugs would be large in size, as they were instantiated as children of the spawner however once the instantiate command was rewritten so that they were not children, they became the correct size. A seperate script then initiates in which the bugs move towards a "Middle" prefab, which is an empty gameobject placed in the middle of the screen. The bugs look at the object and use the MoveTowards function to travel towards it until they are close to the object, at which point the script is disabled with a movement script allowing them to move randomly around the screen is enabled instead. Dragging and disposing of bugs will now need to implemented before the Debugger aspect of the game is combined with the rest of the game.

<a href="https://i.imgur.com/GiKUHqI.png"><img src="https://i.imgur.com/GiKUHqI.png"></a>