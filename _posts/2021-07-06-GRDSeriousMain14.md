---
layout: post
title: Games Research and Development - Bio-Rover Update 11
date: 2021-07-06
excerpt: A more accurate sense of influence, and beginnings of level designing.
tags: [GRD, post, GRDpost]
GRDpost: true
category: post
published: true
comments: true
---
As of now, the LightManager's RayCast has been changed to intersect with the direct outside of the Rover, originally reaching to the middle of the model. This was done through adding the Rover's diameter to the equation (though on first impressions the subtraction of the radius would seem to fit, these led to the RayCast extending further), and as a result the influence placed onto the Rover should hopefully reflect a more realistic reaction from the Rover.

As well as this, initial integrations have begun for the level design, the initial design used the idea of two rows per "theme". From here, the bottom left tile (Dusk Forest) has begun to be fleshed out, with the intent of a small subtle tutorial area developing. This will be done through giving an open area for the player to become accustomed to, alongside some arcs and holed areas umped terrain and for them to practice their movement. However, planning out this layout has revealed that the composite terrain would be extremely large, and thus discussion after the provided session has led to agreement to remove two of the rows, leaving a 4 by 4 grid and in turn still providing a very spacious map even if the tiles are made smaller. Other subjects of discussion that arose from this include possibly using seaweed for scene/tile transitioning, effectively giving the impression of flow and speed to the player (and not only through numbers in a movement script, even making large slow objects seem fast e.g: seeing rocks whizzing by), as well as other important factors on the level layout itself. 

These were oriented around the content of the tiles, ensuring that none are too cluttered and instead spacing tile content out which while making areas seem more barren and sparce, would fit with the more realistic nature of underwater locales and would also encourage exploration from players. As a whole, this would help designate efforts more effectively and could assist in sprucing up the tiles, which in themselves could be populated with or deserted of sealife in areas to make the area more natural and tie together with the more spaced out level features to create a sense of arrival and accomplishment.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=L36BE5oFbCY" target="_blank"><img src="http://img.youtube.com/vi/L36BE5oFbCY/0.jpg" alt="Light Influencing Accuracy and Level Beginnings" width="240" height="180" border="10" /></a>

The initial level layout:
<a href="https://i.imgur.com/8rUy2lF.png"><img src="https://i.imgur.com/8rUy2lF.png"></a>
