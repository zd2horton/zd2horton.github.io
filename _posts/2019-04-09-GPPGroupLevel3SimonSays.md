---
layout: post
title: Gameplay Programming, Group Project Simon Says
date: 2019-04-09
excerpt: The Simon Says puzzle in Level 3.
GPPproject: true
GPPpost: true
tags: [GPP, GPPproject, GPPpost]
category: post
published: true
comments: true
---
The Simon Says puzzle appears at the end of the level. All of the platforms involved are children of an empty gameobject, and if triggered by the player send a flag to the object's script with their Sibling Index. The parent then accesses the child's tag, reading in the colour and after comparing applys a score onto the colour that was stepped on. A check then runs against a list of correct sequence of button hits. If the current state of the puzzle is not listed, it wipes progress and restarts, but continues if the player hasn't won yet. After winning, the door in front of the puzzle then opens. 


<a href="http://www.youtube.com/watch?feature=player_embedded&v=wt_uGHi5GuU" target="_blank"><img src="http://img.youtube.com/vi/wt_uGHi5GuU/0.jpg" alt="Group Project Simon Says" width="240" height="180" border="10" /></a>

The Simon Says cutscene:
<a href="https://i.imgur.com/LwsojBv.jpg"><img src="https://i.imgur.com/LwsojBv.jpg"></a>

Failing the Simon Says:
<a href="https://i.imgur.com/cGnHnIL.png"><img src="https://i.imgur.com/cGnHnIL.png"></a>

Solving the Simon Says:
<a href="https://i.imgur.com/4OX9SWM.png"><img src="https://i.imgur.com/4OX9SWM.png"></a>
