---
layout: post
title: Commercial Games Studio - Potion Panic Update 3
date: 2021-08-04
excerpt: An update on Volcanic Blast, and its implementation.
tags: [CGS, post, CGSpost]
CGSpost: true
category: post
published: true
comments: true
---
As of current, the Volcanic Blast has taken a more complete form. This was undertaken through the use of a Blender created mesh, involving the manipulation of UVs in order to shape into a blast-esque explosion shape. The mesh, using a bottom and a top, was then animated using the size over lifetime aspect of each part with the intention of the blast launching up before sizing out moments later. Once the Standard Assets fire texture was found to be inadequate for the blast, a shader graph was undertaken which initially utilises noise for a rough look, then using UV, time and a speed to help animate it. After this, a colour variable was added to create the material colour, and then a split UV which in turn connects to the alpha and allows manipulation of the material's transparency (allowing for a fading out), then creating the desired explosion effect once applied to a material before the meshes themselves. This finished blast visual was then attached to a working implementation of the spell undertaken by another, this implementation using an outgrowing cylinder to determine damage in an area if enemies are caught in it. Initial balancing efforts for the spell heavily decreased the amount of damage as it was thought to be a multi-hit spell, however this was dropped once the contrary was made clear. A Vector3.Distance method was planned out from this prior state in which the float given would proportionally damage an enemy when appropriate, before likewise being dropped. As the appearance of the cylinder did not match too well with the blast and its mesh thickness was too thick, a new cylinder was created in Blender for use and was given a slightly redder version of the blast material to match with the blast. In terms of work to come, the blast visual may need some adjustments to be more less sudden with the spell, and general maintenance across the projects may also be undertaken.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=oN7M9UmY7Ks" target="_blank"><img src="http://img.youtube.com/vi/oN7M9UmY7Ks/0.jpg" alt="Volcanic Blast Major Update" width="240" height="180" border="10" /></a>