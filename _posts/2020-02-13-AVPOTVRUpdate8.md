---
layout: post
title: Audio Visual Production, OTVR Update 8
date: 2020-02-13
excerpt: Writing code in order to distinguish pathing.
tags: [AVP, post, AVPpost]
AVPpost: true
category: post
published: true
comments: true
---
In terms of smaller progress, the puzzle script for the first scenario has been slightly altered so that when the tree disappears, a tree chopping clip plays to indicate as such. However, in terms of code progress, a basic OnCollisionEnter function has been written to detect hitbox collision (originally intended to use triggers via the ground, however this did not work out), at which point the wagonAudio audioSource will change clips based on the tag of aforementioned hitboxes. While currently the code functions for rock terrain, it does not function for the wooden bridge, so this will need to be looked into.

<a href="https://i.imgur.com/roG0S9I.png"><img src="https://i.imgur.com/roG0S9I.png"></a>