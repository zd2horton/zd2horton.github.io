---
layout: post
title: Commercial Games Studio - Apex Drive Update 6
date: 2021-04-21
excerpt: Creating a concrete elimination system.
tags: [CGS, post, CGSpost]
CGSpost: true
category: post
published: true
comments: true
---
An established method for the implementation of elimination has now been created, building from the current framework while dropping the previously implemented ienumerator. Instead, the code uses a a timer for each vehicle altered using deltaTime before reaching the value of a limit float and dispatching of them if they are still away from view. Initially, this did not function at all due to each if statement checking the boundaries despite being inside of a boundary check which has already been validated as true. This was acting on the logic of if each vehicle checked were its own individual frame, leading to a lack of outcome in both this circumstance and perhaps also the ienumerator due to a loop based logic error. As such, the checks in this context would have proved to be too much and heavily stall the code itself, and consequently removing these unneeded extra checks have resulted in the intended outcome of the code while also making the code more readable. In terms of upcoming progress, a cleaner method of eliminating the vehicles will be implemented in order to link more appropriately with the rest of the codebase and ensure that objects are available for use by the rest of the project if required in any context.