---
layout: post
title: Games Research and Development - Block 0, Rain "Week 3" Update
date: 2021-02-23
excerpt: Summarisation of the progress on the project.
tags: [GRD, post, GRDpost]
GRDpost: true
category: post
published: true
comments: true
---
A long period of time was spent attempting to implement in editor elements for the system, allowing users to toy with the sliders outside of the play mode and possibly save their settings. However, after heavy research into the matter through the Unity documentation and general forums, it was deemed impossible in the manner that was intended unless the entire UI were to be created entirely through code, overturning the current progress entirely. 

As well as this, extensive research into the same areas was conducted to conclude the possibility of implementing a bounding box for the rain particle system, as to give more clarification to the user due to the difficulties of making it out from a distance. Despite this, not much information on the topic was found, with many aspects and features looked into eventually being found as inconsequential for the issue at hand but eventually "Debug.DrawLine" was found. As a debuggin tool, it draws a line from point A to point B with a certain length and with this, a box could be drawn around the system with multiple lines. This did not result in any visually meaningful results however, as lines programmed to draw from the rain system's dimensions did not appear.

With the feedback session, a potential workaround was specified with the editor UI issue. Though making the current UI usable outside of the play mode would be impossible, the idea of making values in the script sliders in the inspector itself was given, and can potentially pave way for an accessible solution to the issue. As for the next workstream, the focus will be "serious games", in which games are used for more serious matters such as scientific data visualisation. This seems to be the next project premise in of itself, and will be prepared for with research on pre-existing examples.
