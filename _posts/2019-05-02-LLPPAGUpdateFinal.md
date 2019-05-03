---
layout: post
title: Low Level Programming, Play and Games Final Update (Post Mortem)
date: 2019-05-02
excerpt: Final thoughts on how the project went.
tags: [LLP, game, post, LLPpost, LLPproject, LLPPAG]
LLPpost: true
LLPproject: true
category: post
published: true
comments: true
---
Overall, our group has made a very functional and complete game. The original game has made a mostly harmless transition to a digitally playable mode and supports four players very well, keeping the game running for the other players should an accidental disconnect occur for a player. The most notable change is the introduction of a board, allowing for a more accessable experience compared to the cards exclusive game from before and also makes more sense for a network reliant game. With this, tiles are a new feature which act in place of picking up cards in turns (a global space will result in the player picking up a global event card, for instance) which further condense the experience into a more understandable one. The game has also increased its number of turns from 10 to 20 as a result of the alterations which now cause the game to become faster paced, but with this players can survive even with no or even negative bits or produce. This in turn can be considered to make the game less suspenseful and action based, but in line with the farming theme makes it a more relaxed experience. Finally, happiness has been modified so that it can add to a player's roll rather than adding to an attacker's dice roll. This is due to attacking as a whole being removed, a mechanic in which the current participating player "bets" up to 5 produce (which are represented by a single die each) in order to take up to the same amount from a target player, the happiness in this context instead allowing the attacker to roll a chosen die up to their happiness number. Due to difficulties as well as balance considerations and overall accessibility, attacking was removed. If the project were to be undertaken once more, it could be beneficial to attempt to reimplement this mechanic albeit in a simpler and more understandable fashion, as it managed to add a level of player interaction both with the game and with other players. These were also the reasons for alterations or removing of global cards such as PETE, Bountiful Harvest, and the Super Shield curiosity card. For the most part however, the game has been remade to a tee.

As the teammate responsible for implementing the game's cards and audio, I managed to come across and use many new aspects of coding. The information for cards is stored in a number of .json files, an idea that I found difficult to implement at first, but attuned to once reading was done around it. This in turn followed with implementing FILEIO in order to read in the files, which felt pleasant to finally be able to learn and use successfully. SoLoud was also new to me, however I did not find implementing it hugely difficult. Rather, the bigger learning experience came from implementing the audio system into the game's service locator for use elsewhere. As well as this, my coding standard has greatly improved as a result of this project and working with others, and using such features as unique pointers and static casts which I had not used before. I feel that working with my teammates has especially helped me in this regard, and has proved to be an invaluable learning experience.

If I were to redo this project, perhaps by myself or with a team, I would focus improvements on the areas I did by general revamps, such as volume settings for the audio rather than muting being the only option. My main area for improvement would be on the code itself, improving formatting as well as learning more about the coding standard so that in the future my programming skills can be good enough to be accepted into industry.

[https://youtu.be/0MzrDsQbDzU](https://youtu.be/0MzrDsQbDzU)

The title screen and menu, as well as a tutorial on how to play:
<a href="https://i.imgur.com/jHisBjd.jpg"><img src="https://i.imgur.com/jHisBjd.jpg"></a>
<a href="https://i.imgur.com/rjXmuAq.jpg"><img src="https://i.imgur.com/rjXmuAq.jpg"></a>
<a href="https://i.imgur.com/bA7w7QK.jpg"><img src="https://i.imgur.com/bA7w7QK.jpg"></a>

The lobby:
<a href="https://i.imgur.com/10ddHIU.jpg"><img src="https://i.imgur.com/10ddHIU.jpg"></a>

In Game:
<a href="https://i.imgur.com/JgY1MzL.jpg"><img src="https://i.imgur.com/JgY1MzL.jpg"></a>

A card in play:
<a href="https://i.imgur.com/K3Dpias.jpg"><img src="https://i.imgur.com/K3Dpias.jpg"></a>