---
layout: post
title: Commercial Games Studio - Apex Drive Update 9
date: 2021-05-19
excerpt: The systems embedded into the main gameplay scene.
tags: [CGS, post, CGSpost]
CGSpost: true
category: post
published: true
comments: true
---
Both the nametags and elimination systems have at least partially been integrated into the level design scene. The nametags' parameters have been altered appropriately for the LevelDesign scene, including offsets, sizes and rotations. Once they were visible and floating atop each vehicle, it seemed that the tags were did not stick out well enough and thus outlines were worked on. Efforts did not seem to result in an outcome however, and after seeing a lack of any after specifying a colour and width, research led to a change in shader for the TextMeshPro being used. As the allocation would have to coded due to all tags being created via script, many solutions were looked into including Shader.Find, Resources.Load, easier access to the appropriate shader as well as creation of a clone font so that the system would be able to set and access the. Though these efforts were not successful, it was realised later on that the TMP's own material and shader were being looked into in the script and not the material and shader of the font, which finally gave in an intended and visually noticeable result through Shader.Find. The Elimination script also works as mostly intended, though just a small amount of the visible screen boundaries seem to count as outside. This will be looked into and solved if it becomes more of an issue, and as well as this giving the tags some flair will also be investigated.