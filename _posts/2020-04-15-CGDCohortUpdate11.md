---
layout: post
title: Commercial Games Development - Cohort Jam Update 11
date: 2020-04-15
excerpt: Bookcases, and a notable rework.
tags: [CGD, post, CGDpost]
CGDpost: true
category: post
published: true
comments: true
--- 
The general code for the vending machine event has now been altered by another in the overall cohort team to be more easily understandable and usable. The most notable change however is that the shaking state for the machine will no longer be used, omitting the need of both visual and audio implementation of the feature. Though it is unfortunate as a way had been figured out to visually show the shaking and was ready to be implemented, this will help streamline the event and the experience to be less ambiguous. To add, the machines now have an animation for falling through usage of SkeletonAnimation and can now also be bookcases, though once again these changes were not performed by the vending machine team. 

Overall, these changes will make working on bug fixing easier thanks to the more streamlined code. In terms of the method planned to be used to show visual shaking, the vending machine script would have instantiated and parented wiggled line sprites indicating shaking, and would instantiated up to three on each side with the state before falling using a ! above the machine with all three lines showing. While this method of visually showing the machine's shakes could attract a player's attention, there could be times where their attention is elsewhere or they are not able to see the signs, which could cause frustration for when the machines finally fall. As the shaking is now removed, the machines are made to fall which as a whole makes the experience more straightforward and creates less uncertainty. 