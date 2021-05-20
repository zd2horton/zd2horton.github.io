---
layout: post
title: Commercial Games Studio - Apex Drive Update 8
date: 2021-05-10
excerpt: Update on the Name Tag progress, and thoughts on individual work.
tags: [CGS, post, CGSpost]
CGSpost: true
category: post
published: true
comments: true
---
As of now, the name tags have been brought to use the direct positions of each vehicle as a destination point rather than converting the positions into a screenpoint set. This has given some notably fine success with the overall intention of the implementation, and the offset has been altered for correct tag placement. However, in tests once Player 1 leaves the others it adopts the Player 2 tag. This seems to be due to Player 2 being the first processed car in the carSystem, consequently creating its nametag first and by extension applying it to Player 1  due to the objects' ordering order. This may require discussion with those involved with processing the vehicles, as it would seem this is an external issue that the Name Tag script is not able to remedy.

As well as this, ideas into the individual work have been crafted. Thoughts of crafting an older platforming title to Unity from scratch alongside new levels were pondered on, however advice has driven away from this due to general time constraints and the exact outcome not being wholly known. This blends into the current solid idea, which draws from a level editor segment the previous idea had and could potentially evolve into a game oriented around the very concept of level design itself. As a more grounded and time efficient concept, a tile based platformer editor could give leeway for multiplayer experiences and possibly even a climber-esque game in which a player would be required to pick up and use various pieces of a level in order to stay airborne. As the best present premise, level design as a game will be looked further into for a more solid idea.