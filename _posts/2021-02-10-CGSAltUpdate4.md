---
layout: post
title: Commercial Games Studio - AltSpaceVR Update 4
date: 2021-02-10
excerpt: Reading more into the MRE SDK and outlining what needs to be done.
tags: [CGS, post, CGSpost]
CGSpost: true
category: post
published: true
comments: true
---
Information on the next workstream has been detailed, with a pool of four existing previous IPs at different points of progress being voted into two ideas for the two groups to take one of. The third workstream will be more open in terms of ideas, and each will soon enough be worked on simultaneously. As for this week's workload, the aim is to reach a creative prototype game, with a basic version running in order to test the difficulty of uploading assets to AltSpaceVR. As such, the Mixed Reality Environment SDK has been looked into, general aspects such as building an MRE and using the Unity Uploader being practiced with. with examples spanning from a simple hello world test to hat assignment and a version of tic-tac-toe. The latter has been especially looked to, as it features a win loss state that would be valuable for the project. Using Java as a base, the code uses an array of victory checks based on all possible winning combinations and ownership of the game squares. With each tile placed, it checks the board state to see if its layout is equal to any of the victory conditions, and if so loads into the victory celebration of the victorious player. As of the moment, the inner workings of the SDK will be looked into, and by the next session at the least a surface level understanding of the coding style should be obtained.