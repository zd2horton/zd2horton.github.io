---
layout: post
title: Gameplay Programming, Group Project Update 2
date: 2018-04-04
excerpt: Current progress, and slight issues.
GPPpost: true
tags: [GPP, GPPpost]
category: post
published: true
comments: true
---
Currently, a door and switch mechanism has been implemented in which once the switch has either been slashed or punched by the player, a cutscene will commence and look over to the door, opening it. The player then has an 8 second timer to go inside, with the door shutting after the timer. However, if the player fails and goes to press the switch again, nothing happens. This seems to be an issue mainly focused on the cutscene code not knowing if the door has shut again, which should be easily fixable soon.


[https://www.youtube.com/watch?v=6t1_kcq68yA](https://www.youtube.com/watch?v=6t1_kcq68yA)
The beginning of the cutscene:
<a href="https://i.imgur.com/5a9QL2G.jpg"><img src="https://i.imgur.com/5a9QL2G.jpg"></a>

The door opening:
<a href="https://i.imgur.com/oA7Tqzv.jpg"><img src="https://i.imgur.com/oA7Tqzv.jpg"></a>