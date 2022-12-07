---
layout: post
title: Low Level Programming, Ex Machina Update 4 (Post Mortem)
date: 2019-02-21
excerpt: The final game, and improvements.
tags: [LLP, game, post, LLPpost, ExMachina]
LLPpost: true
category: post
published: true
comments: true
---
The final game has been finished, and while it is functional, it isn't fully functional. The player moves around the map in a grid like fashion using the arrow keys and can pick up keys using the e key, which open locked doors represented by the yellow lines. The time they have left decreases each time they move, meaning they have 100 moves to complete the map. The final door to Nathan's computer requires a keypad combination, deciphered by a randomly generated binary addition problem. After the player solves this, they can win the game by walking to the computer. 

I was mainly responsible for character movement, the end minigame and handling of sprites, as well as helping in click handling and the logic of the game's keys and doors (which used the previously mentioned array grid movement method). Given the structure of the game, I feel as if the character movement was done well however if I were able to remake the project, I would want the game to have far more fluid movement rather than the retro esque movement required due to the grids being a vital aspect of the game.

As doors were implemented later into development, they seem to have an issue in which they sometimes will not unlock even given the sufficient key. This is a significant problem as it severely hinders play to the point of unplayability, especially if the player is trapped in the first room. A feature such as this would also need to be given a considerable amount of development time in a reattempt so that they can be confirmed as fully working. On the other hand, the inventory system works well as the player is able to pick up the keys placed around the map.

The binary addition minigame implemented generates two random numbers, adding them and storing the result before converting them to their binary alternatives, creating the puzzle for the player to solve. The interface pushes back each number clicked by the player, similar to the input system used in the BASIC Haunted House task, and compares the result with the player's input to determine whether the minigame is cleared or not. I am not sure what can be improved about the minigame, but overall the game would benefit from more minigames in an improvement of it.

I found working with others on the same project an enjoyable experience that I have learned a lot from, especially through sharing code through GitKraken and writing my code to synergise with the code from others in my team. 

Overall, the most important lesson I have learned from this project is to not overthink problems, as doing so can cause the simpler and more efficient solutions to go unchecked. Instead, it seems more beneficial to create working code and then build on from that point rather than head straight for the more complicated methods. This was most noticable with our many attempts to create a different sprite handling system, which could have been circumvented by implementing SpriteComponent and if possible, create a different system from that point. In turn, doing this would have freed up a large amount of time for other aspects of the game, and could have led to a far more complete version.

[https://github.com/UWEGames-LLP-2018/ex-machina-team-sleepy-blind-and-the-robot](https://github.com/UWEGames-LLP-2018/ex-machina-team-sleepy-blind-and-the-robot)

The title screen:
<a href="https://i.imgur.com/h5OV4v7.png"><img src="https://i.imgur.com/h5OV4v7.png"></a>

The player's beginning position:
<a href="https://i.imgur.com/6dZdzHp.png"><img src="https://i.imgur.com/6dZdzHp.png"></a>

Keys being picked up and placed into the inventory system:
<a href="https://i.imgur.com/e6gOPYT.png"><img src="https://i.imgur.com/e6gOPYT.png"></a>

The binary addition minigame:
<a href="https://i.imgur.com/Ia7uHYp.png"><img src="https://i.imgur.com/Ia7uHYp.png"></a>

After the minigame has been cleared, allowing the player to win the game:
<a href="https://i.imgur.com/Swf8F4h.png"><img src="https://i.imgur.com/Swf8F4h.png"></a>

The winning screen:
<a href="https://i.imgur.com/4obhofr.png"><img src="https://i.imgur.com/4obhofr.png"></a>

The game over screen:
<a href="https://i.imgur.com/gGRuqhC.png"><img src="https://i.imgur.com/gGRuqhC.png"></a>
