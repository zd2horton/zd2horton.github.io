---
layout: post
title: Low Level Programming, Text Adventure Game Update 2
date: 2018-11-11
excerpt: Moving the BASIC game into C++.
tags: [LLP, game, post, LLPpost, basic]
LLPpost: true
category: post
published: true
comments: true
---
I have managed to implement most of the game into C++, including events on certain selected spaces, movement and the ability to type commands for the game to read. The data needed for the game such as the items, the rooms and their exits are stored in txt files which are loaded in through fstream. From here, I will need to make general improvements and also include an inventory system in which the player can drop and pick up items, which I will presumably use an array for.

The game running in C++:
<a href="https://i.imgur.com/Ti4KVvN.png"><img src="https://i.imgur.com/Ti4KVvN.png"></a>