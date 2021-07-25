---
layout: post
title: Commercial Games Studio - Apex Drive Update 10
date: 2021-05-22
excerpt: Player identification updates.
tags: [CGS, post, CGSpost]
CGSpost: true
category: post
published: true
comments: true
---
Progress has been made in stylising the name tags, with a custom texture being created for it. This attempts to fit in with the game's atmosphere of expressive vibrant colouring, and helps the text stand out more among the changing environment. The text also incorporates the TextMeshPro Distance Field shader over the Mobile edition, so that the outlines are able to be visualised.

Not soon after this however, talks have discussed the viability of name tags to identify players in a local setting as well as a screen already requiring many UI aspects, touting that they may be widely unnecessary and possibly not quick enough an identifier in such a setting. Though nametags would be notably useful online when playing against others, most in the group agreed a more fitting local implementation of player identification would be visual indicators such as different colours. These would be far easier and simpler for the mind to visualise, understand and deduce, thereby proving to be a more efficient method at least for local play. With this, the most optimal way for the result to be reached would be for the roofs of the vehicles to be allocated different colours for each player, being done in script through the alteration of the vehicle model's roof material (as to accomodate for additional or low player counts).

Due to the structure of the model and gameobject holding it, the model itself is a sibling of the PositionUpdate object that the script was required to access through the PositionUpdate object's parent in a GetChild statement. Once the required material for altering was declared, the colour would then have to be changed depending on the player number with a switch case performing this as a result. Using a simple material.color change did not work however, and contextualised statements such as material.SetTexture also provided a lack of outcome before changing the shader or material's "_BaseColor" through material.setColor (as the intent was to change the "Base Map" colour in the material's surface options) managed to give the intended result.