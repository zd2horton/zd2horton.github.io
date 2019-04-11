---
layout: post
title: Low Level Programming, Play and Games Update 2
date: 2019-03-20
excerpt: Further developments on reading card data into the game.
tags: [LLP, game, post, LLPpost, LLPPAG]
LLPpost: true
category: post
published: true
comments: true
---
After more development time, the .dat file has been converted into different .json files for easier reading. Using nlohmann json caused the dat file to return an abnormally large number of errors, all concerning formatting. As a result, rather than using a json style format, the dat file was transformed entirely into a json file however this had to be split as it would not accept the card data as one file, returning more syntax errors.

This can benefit the game mostly due to the fact that using multiple json files, one for each card type, can allow for easier reading and as a result easier multiplication of each card. As well as this, json file reading has been implemented with the system opening a FILEIO buffer in order to read the data in, then outputting it into a readable json structure. As a test run, the program can read in one card currently but before long it will be able to read in each player's deck.

The "Scorched Earth" dragon card being successfully read in:
<a href="https://i.imgur.com/qPM4dCM.png"><img src="https://i.imgur.com/qPM4dCM.png"></a>
