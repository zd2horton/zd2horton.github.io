---
layout: post
title: Low Level Programming, Play and Games Update 5
date: 2019-04-05
excerpt: Adding the global deck system. 
tags: [LLP, game, post, LLPpost, LLPPAG]
LLPpost: true
category: post
published: true
comments: true
---
The global deck for the game (including global, curiosity and sabotage cards) has now been implemented. Unlike the previous decks however, the global deck has been implemented into the server side. This is because the global events will affect all players, meaning it is more appropriate to host them on the server rather than the server having to try and fetch the data from all clients. While FILEIO, an ASGE method, was used to load the previous decks into the game, its absence in the server codebase means that ifstream was used to load the json files. As well as this, game.dat is also unusable in the server side of operations, so the data folder containing the card json files used to create the global deck needed to be added to the bin of the GameServer make so that the server is able to access them. From here on out, the process is similar to the previous in which each card is initialised as many times as the global deck needs, and shuffles once all cards are added to the deck.

The global deck implemented, using 80 cards (16 global, 32 curiosity, 32 sabotage)
<a href="https://i.imgur.com/qqY9zOt.jpg"><img src="https://i.imgur.com/qqY9zOt.jpg"></a>
<a href="https://i.imgur.com/e03kvM9.jpg"><img src="https://i.imgur.com/e03kvM9.jpg"></a>