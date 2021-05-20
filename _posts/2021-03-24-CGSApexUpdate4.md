---
layout: post
title: Commercial Games Studio - Apex Drive Update 4
date: 2021-03-24
excerpt: Progress with the elimination system.
tags: [CGS, post, CGSpost]
CGSpost: true
category: post
published: true
comments: true
---
Currently, efforts geared towards Apex Drive's elimination system are underway. Methods to have an object disappear based on their visibility with the camera are the primary focus, with OnBecomeInvisible being the most prevalent solution upon researching. However, this function seemingly works differently in the Unity editor compared to a finished and compiled game, thus giving the need for a different solution so that visual progress can be seen. As well as this, another method attempts to convert an object's world co-ordinates into viewport co-ordinates, then checking for these co-ordinates to be outside the boundaries before the code goes to destroy the object. Neither of these methods have encountered any visual result as of current, but will be continue to be built upon. 
