---
layout: post
title: Games Research and Development - Block 0, Rain Update
date: 2021-02-09
excerpt: An update on implementation, as well as other notes on the course. 
tags: [GRD, post, GRDpost]
GRDpost: true
category: post
published: true
comments: true
---
Overall, the emphasis on the more written side of the course has increased, detailing such aspects as the project report needing to take the shape of an academic report paper in a journal, detailing the problem tackled before summarising research and then reflecting on areas of technical innovation in the project. With this, the prototype will be assessed on its design, quality, implementation and general success in meeting stakeholder requirements and proving its usefulness. Following on from this, short video logs as well as documentation will detail the methods to approaching and designing the project, as well as stakeholder engagement (such as regular minuted meetings) and aspects resulting from said engagement.

For the current project at hand, a GUI mimicking the prototype was recreated in Unity early on, using an example particle effect in order to show each setting's effects. The current framework of implementing the features has come from assigning a value to the particular UI piece in OnGUI, allowing it to fluctuate depending on the user's selections. These values are then applied to the appropriate aspect about the particle system in the Update function. For this, variables were used in order to access the features needing to be changed by the UI settings, as directly calling for them to be altered was not possible and would be a more hardcoded approach. Though most UI options have been coded through this method, a handful such as radius, droplet shape and a splash toggle will require more overall context from other aspects of the project in order for initial implementation to take place. As well as this, various small alterations have been made in order to make some options more appropriate, including the separation of the rain's intensity and concentration and the addition of an Alpha slider for drop transparency.

Concerning how the script acquires each UI element, the method used currently involves a serialised field for them, meaning that while they stay private there is an option to drag each element in as if the variables were public. Due to the nature of the system at hand, this is not a very practical method of acquisition and thus a cost effective method of allocating the elements privately will become a major aspect to research on. For instance, while GameObject.Find or FindWithTag allow for a more private, precise process, they are extremely cost ineffective and would challenge compatibility with lower end machines if applicable. 

Currently, as the method used to alter the rain's settings is notably basic, a number of issues to address will include researching a more efficient, streamlined and possibly complex implementation overall, the inclusion of the prior missing settings and an alteration to the colour settings, as the use of the element in the particle system looks to be far simpler than initially prepared for. To add to this, the system could also be made so that it works with multiple systems across the board, and possibly even be accessible outside of the play scene.