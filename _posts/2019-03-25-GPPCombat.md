---
layout: post
title: Gameplay Programming, Melee Combat
date: 2018-03-25
excerpt: Combat with large slime enemies.
GPPproject: true
tags: [GPP, GPPproject]
category: post
published: true
comments: true
---
The final individual task requires combat against a "large gelatinous cube". This cube patrols around until it sees the player and homes in, hopping and attacking by bumping into the player before retreating backwards. The initial slime takes 3 hits before dispersing into 2 smaller slimes, which take 2 hits themselves in order to break into 1 hit very small slimes.

The initial, large slime implemented patrols around a designated spline while calculating the distance between it and the player. Once the player is close enough to the slime, it breaks out of the spline and moves towards the player, beginning to play boss music. From time to time it will also bounce at random, getting closer to the player and if touching them, it waits two seconds before moving to a retreat zone in the corner quicker than its initial chase speed for another 5 seconds and moving towards the player once more. If it manages to push both itself or the player off the battle platform, both entities will respawn based on whether they fell off or not. 

The slime will also check if the player is attacking, the initial implementation checking if the player has flipped into the slime while the newer implementation checks for a punch. If so, it plays a damage sound effect and reduces the total amount of HP, beginning a small cooldown before the player can hit them again. If the slime has no more health, it will shrink rapidly and instantiate 2 smaller versions of itself around itself (unless it is a 1 HP slime) before disappearing. Once the player has eradicated the slimes, the game is over and the player wins.

The initial way to damage the slimes was by checking the animator's current state, running a comparison on if it was currently in the double jump flip animation. Due to the uncertainty of the double jump's state in the animator, as well as the smaller stature of the slimes after the first and precision required, this was a very unreliable method. However, not soon after, the slime was able to be damaged via punching, as previously double jumping was used as an alternate to this as it had previously been unable to be implemented. This made the combat a lot more reliable and enjoyable, as hitting the slimes felt less of a probability and more of a certainty.

Overall, however, the slimes themselves could use improvement. The patrolling used could be randomised further in order to give them more life, and this can also factor into the retreating where the slime could run away to a random spot rather than a designated corner. The biggest problem is with the smaller slimes, as their behaviour seems completely dysfunctional. They do not move towards the player at all, and touching them does cause them to try and retreat but not to much success. I am unsure of how this issue occurs.

[https://www.youtube.com/watch?v=UeyefiVz9X4](https://www.youtube.com/watch?v=UeyefiVz9X4)

The slime following a spline:
<a href="https://i.imgur.com/3Yzk7rU.jpg"><img src="https://i.imgur.com/3Yzk7rU.jpg"></a>

The slime jumping towards the player:
<a href="https://i.imgur.com/xsQMcz4.jpg"><img src="https://i.imgur.com/xsQMcz4.jpg"></a>

The slime retreating to the corner:
<a href="https://i.imgur.com/SiCgZI3.jpg"><img src="https://i.imgur.com/SiCgZI3.jpg"></a>

A medium slime shrinking after having punched it:
<a href="https://i.imgur.com/ypRWGpj.jpg"><img src="https://i.imgur.com/ypRWGpj.jpg"></a>