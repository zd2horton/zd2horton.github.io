---
layout: post
title: Games Research and Development - Block 0, Rain Update
date: 2021-02-16
excerpt: An update on implementation, as well as other notes on the course. 
tags: [GRD, post, GRDpost]
GRDpost: true
category: post
published: true
comments: true
---
After extensive research into the topic through the general Unity documentation and queries surrounding implemenation was undergone, it has been shown that particle colouration uses values from 0 to 1 in code for RGBA elements instead of 0 to 255. As a result, this range was initially used for all values but a general lack of visual aid on each colour for users as well as confusion for any looking into the code led to the implemenation of a visual showing each colours' value from 0 to 255, with the code converting these numbers appropriately. Since it was found through testing that 0 would lead to black and 1 would lead to white, it made sense for the slider values to be altered as 0 to 255 for clarity while the startColour values would take the aforementioned slider values and divide them by 255 in order to acquire the intended data. Input fields were initially considered and attempted for implementation alongside the sliders but ultimately the idea was dropped. This was due to that fact that the system would have to choose a prioritising method of colour assignment, which in turn proved either the slider or field redundant as the values for either would be reset in order to match the other. GUI boxes have been used in order to show the colour values to the user, currently however the boxes appear in a reverse order and appear far away from their respective sliders despite the code calling for them to be spawned next to them. The cause of this is unknown but much like the overall implementation of the system, this will be heavily looked into.

As for other information explained, suggestions have been made for the system to be made like a pipeline, with the rain potentially being editable in the edit mode and being loadable and saveable. This would increase the usefulness of the system notably, as it would potentially remove the need to play the scene each time the rain needs to be edited. This feat should not be difficult to implement, due to previous experience acquired with loading and saving particular data to a file.
For the overall presentation, an overview of the period of implementation and research should be given with a summarisation of what has been attempted in implemenation. As well as this, a live playable demo of various aspects working together should be present, with a video for if things go wrong.