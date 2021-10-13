---
layout: post
title: Creative Technologies Master Dissertation Update 9
date: 2021-09-21
excerpt: Attempting to create a model, and supervisor advice.
tags: [CTMD, post, CTMDpost]
CTMDpost: true
category: post
published: true
comments: true
---
As of current, an agent to control the player is being looked into for creation. This involves declaring required aspects of the project in the Initialise function, redeclaring those that are to be reset in OnEpisodeBegin (position for example), and picking up various information from factors the agent requires knowledge of in CollectObservations, and applying agent input to the horizontal and jump variables in OnActionReceived as well as deciding which actions require increasing or decreasing in reward. These in turn relate to the behavioural parameters, with vector space size increasing in one for each value collected (two Vector3 values and a float requiring a space size of seven), the defined continuous or discrete actions in the script deciding the parameter's nature (and discrete branches needing a size proportionate to each value the branch can cover), and the behaviour type being dictated via the prescience or absence of a Heuristic function. As well as this, in order to help with the Heuristic and potential agent controls, jumping has also been reworked to be toggled from an external boolean rather than directly using the Input class.

In addition, a meeting with a new supervisor has condensed the scope of the project some more due to factors such as overall time remaining, complexity (highlighting level creation rules and intricate human level quality content as some reasons) and lack of general examples in the specific subject area of platformers. The project has hence been scaled down to focus more on user testing and a potential AI implementation, in which a number of metrics of successful level design (engagement, enjoyment, etc.) are to be researched in a small number of pre-made levels. The aforementioned AI implementation will use an ML-Agents built agent in order to complete these, with its overall effort (time, potential item collection) being paralleled with players' own playtests in order to find potential correlations (such as if the time taken for the AI to fully complete a course could correlate with player engagement, or if it would find a level as difficult as a player would). This in turn creates a new hypothesis looking into the effectiveness of an AI agent in playtesting, and consequently a total of three levels are to be created. These include elements that will increasingly test both the player and AI, requiring more complex inputs in later segments that the AI would need to adapt to (also including optional items and segments to provide quantifiable factors for comparison).

<a href="https://i.imgur.com/xICeyok.png"><img src="https://i.imgur.com/xICeyok.png"></a>