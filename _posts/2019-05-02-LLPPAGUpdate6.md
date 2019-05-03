---
layout: post
title: Low Level Programming, Play and Games Update 6
date: 2019-05-02
excerpt: Implementing the game's audio.
tags: [LLP, game, post, LLPpost, LLPPAG]
LLPpost: true
category: post
published: true
comments: true
---
Audio for the game has now been fully implemented, including music (for the menu, lobby and gameplay states) and a number of sound effects. SoLoud has used, with a class housing each sound and the SoLoud system, which is used to initialise each sound into memory. Access to the audio engine is then handed over to the game's service locator through usage of pointers and unique pointers, initialising it in context of the game and allows all client code to use it. If the code wishes to play a sound or play an audio track, an enumerator is used in conjunction with a play function which detects via a switch which sound the play function needs to play. There is also a similar stop function in order to stop a track from playing, and a mute button which will mute all audio playing.

[https://youtu.be/WSW6GD6W81w](https://youtu.be/WSW6GD6W81w)