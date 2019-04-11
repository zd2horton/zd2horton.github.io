---
layout: post
title: Low Level Programming, Play and Games Update 3
date: 2019-03-22
excerpt: Card sprites implemented, as well as drawing and shuffling.
tags: [LLP, game, post, LLPpost, LLPPAG]
LLPpost: true
category: post
published: true
comments: true
---
The card system now has an initialising function in which it will create a deck (represented by a vector) for the given species. As well as this, sprites are now implemented with each card, as each sprite file name shares the name of the card allowing for easier loading through the pre-existing card name variable retrieved from the json file.

When a deck is initialised, it will initialise 3 of each of its species card in turn before creating 3 of each general card, resulting in a 21 card deck for each player and shuffling itself after. There are also functions to draw a card (returning the card element in front of the vector) and pushing back a card into the deck vector in order to "return" it. As the dragon deck was used as a test, the rest need to be added as well as the global card deck (global, curiosity, sabotage).

Shuffling implemented into the dragon deck:
<a href="https://i.imgur.com/ZTti9dK.png"><img src="https://i.imgur.com/ZTti9dK.png"></a>
