---
layout: post
title: Commercial Games Development - Foundary Frenzy, Update 2
date: 2019-11-05
excerpt: The status of the project before presentation.
tags: [CGD, post, CGDpost]
CGDpost: true
category: post
published: true
comments: true
---
The Debugger is now fully implemented into the overall game. As well as this, dragging and disposing of bugs is also a feature. This is done through a script that translates the user's touch positions into world point co-ordinates (originally mouse co-ordinates) and applies the difference between them and the position the position was clicked down at in order to have the bug dragged along. The bug is then disposed through colliding with a bin prefab while it is being dragged, which then adds to the total score. Some issues arose, the most notable of which involved bugs rotating strangely in a 3 dimensional manner. This was fixed by freezing rotation, which then created an error in which bugs could potentially fly off at high speeds if they collided with one another. Altering the movement scipt fixed this however, and any outliers that could potentially arise from this are destroyed if they travel outside the boundaries of the screen.

In the context of the game, the Debugger is used by spawning bugs in the middle of the screen (with the spawner now directly in the screen's middle, invisible and still able to spawn bugs in controlled random positions) and having them roam shortly after due to the "middle" prefab being close by to the spawner. The players must then dispose of bugs by dragging them into the nearby bin before they interfere with the other games by blocking the players' views and touch commands. Initially, 2D values such as 2D collisions and 2D vectors were used, however these were connected to 3D in order to comply with touch controls. The overall final game has players working in the Foundry playing three separate mini-games at the same time: the Debugger, in which they're required to dispose of bugs in order to properly create robots requested of them from parts in the "Robot Builder" minigames, while avoiding obstacles with their drone in "Drone Runner". While Debugger can span the entire screen if bugs are unattended, each game takes equal space on the screen and require different touch controls (dragging, touching swiping) which helps make the gameplay feel less stale. 
<a href="https://i.imgur.com/0yYNlCO.png"><img src="https://i.imgur.com/0yYNlCO.png"></a>