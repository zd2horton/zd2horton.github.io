---
layout: post
title: Gameplay Programming, Group Project Reactive Platforms
date: 2019-04-09
excerpt: Implementation of reactive platforms in Level 3.
GPPproject: true
GPPpost: true
tags: [GPP, GPPproject, GPPpost]
category: post
published: true
comments: true
---
At the level's beginning during the player's travel to the door, they must step on platforms guiding them there. In order to detect the player, an additional and taller box collider was added. From here, if a platform is stepped on then a boolean is set to true, but set to false if the player leaves the platform. While it is being stepped on, it moves down gradually to a set amount before stopping, and once stepped off of, the platform will slowly return to its original position.


<a href="http://www.youtube.com/watch?feature=player_embedded&v=1yAt0jrCz4s" target="_blank"><img src="http://img.youtube.com/vi/1yAt0jrCz4s/0.jpg" alt="Group Project Reactive Platforms" width="240" height="180" border="10" /></a>

A platform being stepped on and weighing down:
<a href="https://i.imgur.com/JLW3hGM.jpg"><img src="https://i.imgur.com/JLW3hGM.jpg"></a>

The platform moving up due to the weight leaving:
<a href="https://i.imgur.com/EGbcfLg.jpg"><img src="https://i.imgur.com/EGbcfLg.jpg"></a>

Simon Says platforms:
<a href="https://i.imgur.com/M0hfNuo.jpg"><img src="https://i.imgur.com/M0hfNuo.jpg"></a>
