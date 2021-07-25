---
layout: post
title: Commercial Games Studio - Potion Panic Update 2
date: 2021-07-21
excerpt: Tending to the first of Potion Panic's spells.
tags: [CGS, post, CGSpost]
CGSpost: true
category: post
published: true
comments: true
---
Currently, a start has been made on implementing Volcanic Blast. This is a spell that damages via proximity of its usage, and is given a total of one use. A particle system has been created for it, with the initial implementation of OnCollisionEnter not seeming to work. This could be due to its particle system like nature, and thus it may be more appropriate to use a particle system based OnCollisionEnter in the player's script rather than OnCollisionEnter on the system's side. As well as this, an overlap based implementation may also work.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=sWprqXB5DPY" target="_blank"><img src="http://img.youtube.com/vi/sWprqXB5DPY/0.jpg" alt="Volcanic Blast Update" width="240" height="180" border="10" /></a>