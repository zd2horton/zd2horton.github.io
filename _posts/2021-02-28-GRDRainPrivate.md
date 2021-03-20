---
layout: post
title: Games Research and Development - Block 0, Rain Privatisation
date: 2021-02-28
excerpt: An explanation of the script's privatisation.
tags: [GRD, post, GRDpost]
GRDpost: true
category: post
published: true
comments: true
---
As of now, the script for the rain system UI has now dropped the need of serialised fields resulting in a script that users merely need to place on their systems without dropping in various UI elements like before. This was implemented once stepping back and looking into the issue before realising that the UI elements were usable as the canvas children and therefore accessible as such. This gave way for the use of GetChildren which in turn allows for the dealing of the elements privately. Though the straightforward assignments of the elements seemed unappealing initially, more research was done to see if a line effective method could be substituted for it whether this would be a struct or array to group the elements into. This was ultimately not possible for the entire set of elements, but the method was consequently adopted with the multi element aspects such as colour assignment in which the parent gameobject is accessed and iterated through in order to fill UI arrays with the resulting elements. Though GameObject.Find was previously mentioned as undesirable, a single usage of it in the start function seems to not be too costly while also helping supply the code with the resulting branches needed to acquire the UI elements. To add to this, a new colour slate has been implemented as to fit appropriately with the new coding (making use of as few GetChildren statements as possible) and improve overall presentation and accessibility, as the alpha slider handle would at times compromise itself and be far less visible if the alpha value is low.

https://dev.to/andytq/unity-comparison-of-performance-cost-between-gameobject-find-and-direct-referencing-pb