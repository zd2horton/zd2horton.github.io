---
layout: post
title: Low Level Programming, Text Adventure Game Update 1
date: 2018-10-28
description: Developments on the Text Adventure BASIC game.
tags: [LLP, game, post, LLPpost]
LLPpost: true
category: post
published: true
comments: true
---
I have compiled and run the BASIC game a number of times, taking notes on the results of such. Some aspects of the game are very buggy, one of which was a simple fix. Beforehand, the ghosts in the Upper Gallery room were not appearing due to their flag not being initialised as such to set up their appearence, fixed by altering Line 2090 so that flag 27 is set to on. Other bugs include the game's boat not appearing consistently and "xzanfar" having a double use in teleporting the player to the Dark Corner room though I do not know what is causing either of these.