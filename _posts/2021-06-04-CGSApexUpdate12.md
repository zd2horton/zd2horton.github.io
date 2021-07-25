---
layout: post
title: Commercial Games Studio - Apex Drive Update 12
date: 2021-06-04
excerpt: Creating UI bars for the project.
tags: [CGS, post, CGSpost]
CGSpost: true
category: post
published: true
comments: true
---
As of current, basic UI bars have been implemented. A prefab canvas contains four bars, each with a border and inner bar (the latter of which has been given a slider property as to function the bar properly). Text objects are also present, but these are only for further implementation once a solid ranking can be calculated. Through a created Bar script, these components as well as a gradient are declared and allocated. Through slider manipulation, the powerAmount from the pre-existing Abilities script in each vehicle is used and alongside this, affects the slider's colour due to the aforementioned Gradient. However, this only currently shows one colour at one time, and a bar with the gradient flowing through it is closer to the intended goal. This is being heavily researched into, and should be implemented soon alongside proper ranking portrayal.