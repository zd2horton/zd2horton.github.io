---
layout: post
title: Low Level Programming, Text Adventure Game Final Update (Post Mortem)
date: 2018-11-15
excerpt: Final thoughts on the Text Adventure Game, and the finished product.
tags: [LLP, game, post, LLPpost, LLPproject, basic]
LLPpost: true
LLPproject: true
category: post
published: true
comments: true
---
Overall, I believe that the final game I have created is satisfactory. The game is a remastering of the original BASIC game, with a little more personality in the player's interface and irons out various problems the game had in its BASIC reincarnation, such as a previously mentioned bug in which using the Xzanfar spell would cause teleportation. 

The main frame of the game takes the input from the player, pushing back each character into a string array which is then broken down and processed by a multitude of if statements to detect if the player's input is a legal action, after which the program will jump to the appropriate function where action can be taken. 

Flags from the BASIC version are operated in this version via an enum of bools, two of which represent a win condition and a fatal condition (in which the player cannot escape, for instance if the player meets the bats without aerosol or the ghosts without batteries to power the vacuum), the latter of which was not in the BASIC build. As a result of this, the player is now able to see when the game is over rather than be unknowing and stuck in a room with no solution.

Finally, the player's inventory has been coded using a vector which is an element similar to an array but is dynamic in size. I found using this stucture for the first time very intuitive and useful, as functions allowing the addition and removal of items in the player's inventory were able to be coded without many problems.

However, there are many aspects I could improve on overall. I believe that I could have used a larger number of classes outside of the game's items, rooms and possible actions and also allow the data of said aspects to be loaded in a more proper fashion. While FILEIO was an available choice, I was not able to understand it very well and as a result I opted for fstream instead. As FILEIO is the more efficient and cleaner option, I should attempt to place more time into learning it.

To add, the code's structure could also be optimised, mostly the way in which the user's input is handled. The code first checks if the input contains more than one word, and then checks if a given verb is correct before the appropriate function checks (if applicable) the noun is also correct. This process relies on an extremely large amount of if statements, which is a very inefficient coding method and would not be accepted in an industry standard project. Resultantly, it is vital for me to improve my coding method as to avoid such a case like this again.

[https://github.com/UWEGames-LLP-2018/basic-reb0rn-zd2horton](https://github.com/UWEGames-LLP-2018/basic-reb0rn-zd2horton)

The player being locked in:
<a href="https://i.imgur.com/LvWzf4I.png"><img src="https://i.imgur.com/LvWzf4I.png"></a>

Finding the key after examining the coat:
<a href="https://i.imgur.com/fy7jZIR.png"><img src="https://i.imgur.com/fy7jZIR.png"></a>

An example of an incorrect input:
<a href="https://i.imgur.com/As033cs.png"><img src="https://i.imgur.com/As033cs.png"></a>

Use of the inventory system:
<a href="https://i.imgur.com/sKRv9uW.png"><img src="https://i.imgur.com/sKRv9uW.png"></a>

An example of a death screen:
<a href="https://i.imgur.com/QVKdPtf.png"><img src="https://i.imgur.com/QVKdPtf.png"></a>