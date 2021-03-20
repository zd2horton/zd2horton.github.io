---
layout: post
title: Games Research and Development - Serious Games Idea Update 4
date: 2021-03-19
excerpt: The fortunate implementation of data collection and loading.
tags: [GRD, post, GRDpost]
GRDpost: true
category: post
published: true
comments: true
---
As of now, data loading and collection from online resources is now fully functional without issue. This was done via the use of the previously created ParliamentData data structure directly in the loading script rather than the external method, giving a more direct level of access. For an unknown reason this let the code bypass the previous errors from before, and once this stage was reached the only remaining issue was that of an input string incorrect format error with the parsed integer values. However, int.Parse was able to be substituted with int.tryParse, resulting in a successful implementation.
16


<a href="https://i.imgur.com/pjOgivO.png"><img src="https://i.imgur.com/pjOgivO.png"></a>

<a href="https://i.imgur.com/p1xDvGF.png"><img src="https://i.imgur.com/p1xDvGF.png"></a>

<a href="https://i.imgur.com/WflfYjz.png"><img src="https://i.imgur.com/WflfYjz.png"></a>