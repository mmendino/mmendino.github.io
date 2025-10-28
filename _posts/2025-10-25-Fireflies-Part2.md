---
layout: post
title: Simultaneous Fireflies
subtitle: Combining firefly patterns to one code!
tags: [Arduino, state-based variables, fireflies]
author: Melissa Mendino Solano
---

Part 2 of the Midterm project! For this part we had to make the fireflies all run in one file, to have them run on the lilypad at the same time. This was honestly pretty straightforward since I used a state-based approach for Part 1, and all I had to do was make sure that all of my variables were on top and that the correct information was under setup and loop.

I used the same code for the flashbulb and synchronous fireflies, but edited the code for the big dipper to make it increase non-linearly. I also added a new firefly pattern - the blue ghost firefly! The blue ghost firefly brightness goes up or down randomly every half a second, by 50, never fully turning off and going doing when it reaches max brightness. 

Here is a picture of my fireflies turning on, although I could not get a picture of them all on at the same time! 

One hint for others: When trying to do the blue ghost firefly, make sure you define what the the random generated number will do! I tried multiplying the 50 by the random number generated to make it go up or down, but it simply added zero to the brightness or added 50 to keep going up because it only generated numbers 0 and 1. It took me a while to notice that that was the issue so make sure you are stating what you want the 0 and 1 to do. 
