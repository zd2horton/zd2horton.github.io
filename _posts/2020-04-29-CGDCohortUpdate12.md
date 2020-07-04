---
layout: post
title: Commercial Games Development - Cohort Jam Update 12
date: 2020-04-29
excerpt: A small fix for dying pawns.
tags: [CGD, post, CGDpost]
CGDpost: true
category: post
published: true
comments: true
--- 
A recent bug in which a fallen machine would kill pawns has been fixed. This was initially caused by a restricted accessibility to turning "canCrush" to false, which is used when true to kill pawns. Thus, the initial idea was to use a co routine to make the Boolean false when required, but was passed over due to a pre-existing coroutine being used to change canCrush to true. Eventually after not being able to draw any more methods of fixing the issue, a coroutine was implemented and now works as intended. Another issue now needs to be addressed in which pawns can pass through fallen machines, and after reviewing the vending machine code and general discussion it has been concluded that it seems to be an external problem with all props. Currently it is uncertain on how to fix it, but it seems that as it is listed as a general issue it will be discussed more soon.


<a href="https://i.imgur.com/PAqQOc3.png"><img src="https://i.imgur.com/PAqQOc3.png"></a>