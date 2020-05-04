---
layout: post
title: Audio Visual Production, OTVR Update 7
date: 2020-02-06
excerpt: Progress on audio based post-processing.
tags: [AVP, post, AVPpost]
AVPpost: true
category: post
published: true
comments: true
---
Currently, audio post-processing is progressing more for the first scenario. Ambience required such as fire crackling and wagon noises have been implemented, and the next step is to implement wagon sounds for when the cargo travels on the bridge and rock areas in the scenario. This will require extra scripting in order to implement.

The implementation uses a plugin named ONSP Audio Source, which helps spatialize the audio in the VR setting. From the experience of using it so far, the range seems to be the primary factor in how far away the audio can be heard, and the volumetric radius involves how loud a sound will be depending on the distance inside the range. This may be incorrect, but seems to be the case for the moment. 

<a href="https://i.imgur.com/fKyK6sI.png"><img src="https://i.imgur.com/fKyK6sI.png"></a>