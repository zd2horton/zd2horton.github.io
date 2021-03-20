---
layout: post
title: Games Research and Development - Serious Games Idea Update 3
date: 2021-03-16
excerpt: Tribulations of implementing data loading.
tags: [GRD, post, GRDpost]
GRDpost: true
category: post
published: true
comments: true
---
As with before, the majority of the focus this week was on data collection and processing. A large amount of progress has been made on this, but a small push still needs to be made for full functionality. Multiple methods were looked into and attempted, including the separation of the data structure into a seperate CS file, creation of the data structure in the loading code itself, and various arrays that could fit the requested data.

For the first method targetting the JSON data structure, an overall reading in of the data was successful however the complex structuring of the data as well as the previous issue of layered json collections resulted in a large amount of difficulty in transferring the stream into the local data structure.

As a result, other methods were looked into after this and from here the notion of using a CSV file was decided on. Though as previously mentioned there are no integrated functions for the format such as JsonUtility, each entry having its own line and each attribute being easy to separate from the rest of the line made it appealing to at least attempt to use the format. As such, a CSV oriented collection of data was used, with an appropriate class going over its attributes. 

With both the JSON and CSV implementations, an APIRequest was created out of the target URL before a Response is acquired from it, a StreamReader then picking up all of the data from the response's stream. While the JSON's method tried using the JsonUtility method in order to format data, this was unsuccessful as mentioned. 

Meanwhile, the CSV's method reads each line of the stream until the end, splitting the current line into a string array and assigning each element of it appropriately into the data structure one by one. While this process does not make the code look very appealing due to a large amount of allocation, it is currently the optimal and most functional way compared to the others until a suitable loop based method is found and implemented (incorporating both the string and integer data). Though on paper this should be successful, it is currently held back by an unset object reference error of unknown cause, despite the code implicitly declaring the data array beforehand. With some tinkering this error converts into one of invalid scope, however overall these will need to be addressed in order for the data reading to advance.


<a href="https://i.imgur.com/nf2vec9.png"><img src="https://i.imgur.com/nf2vec9.png"></a>

<a href="https://i.imgur.com/fkpBiE2.png"><img src="https://i.imgur.com/fkpBiE2.png"></a>

<a href="https://i.imgur.com/V8u92Q2.png"><img src="https://i.imgur.com/V8u92Q2.png"></a>