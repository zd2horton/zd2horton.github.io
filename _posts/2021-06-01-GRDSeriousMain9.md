---
layout: post
title: Games Research and Development - Bio-Rover Update 6
date: 2021-06-01
excerpt: Working on an energy depleting system.
tags: [GRD, post, GRDpost]
GRDpost: true
category: post
published: true
comments: true
---
As the Rover's energy could dwindle, a system is now being worked on to reflect this. In order to lay the groundwork, a foundation has been created in which the Rover's energy begins at 100, and decreases through DeltaTime until it matches 0. This in turn affects the torque added to the Rover's Rigidbody, as the Rover Energy variable is now a factor and altered accordingly so that as the energy depletes the Rover consequently moves slower until coming to a stop. However, as previously clarified in the client meetup, this could cause disengagement with the overall game and thus alongside this another method has been implemented in which the screen darkens, hampering the player's view moderately. This was achieved through creating a Canvas holding a black screen image, initialised to be transparent before DeltaTime gradually increases the alpha channel's value. In order to optimise the system somewhat, it was then made so that any of these alterations would only be undergone if the player is moving as otherwise they would presumably not be using energy. For future improvements, refinements once the project has been developed further as well as context will assist in optimising the system.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=6GOwVPDXlcU" target="_blank"><img src="http://img.youtube.com/vi/6GOwVPDXlcU/0.jpg" alt="Energy Depletion System Update" width="240" height="180" border="10" /></a>