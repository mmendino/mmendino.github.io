---
layout: post
title: Separate Fireflies
subtitle: Programming firefly flashes using state-based variables
tags: [Arduino, state-based variables, fireflies]
author: Melissa Mendino Solano
---

This was part 1 of a midterm project! Using a state-based approach (instead of a sequential one) I had to create a program for each of 3 different firefly flashing patterns. While the flash bulb and big dipper patterns were not easy, the hardest of them was the synchronous pattern!

The point of using a state-based approach, which is super hard btw, is to be able to program mulitple things at the same time without having a delay for one that doesn't work for another one. The sequential approach depends more on delays to determine when to do something, but is more straightforward if you know what the behavior needs to be. State-based however requires you to figure out what states you need to catch at the beginning of the state or to update a variable.

The flashbulb firefly only needed to catch start on, and to catch start off. I had to catch start on every 4 seconds and start off every 500 seconds. Here is a picture of the light on while the timer ran!

The big dipper firefly had to catch start on, catch start off, and catch increase brightness! I had to create a variable for brightness since brightness had to increase every 100ms and then turn off when it reached max brightness. I also had to create a variable for how much to increase brightness (fadeAmount) and when (increaseTime). Here is a picture of it while it is on and increasing in brightness!

The synchronous firefly had a lot more states to catch! The pattern was to flash three times quickly every 10 seconds, with a different amount of time on than the handout. I had to catch ON at the beginning, Off at the end, off during the phase, and on during the phase as well as updating other variables needed to determine if it was inPhase, how many times it had flashed (synchCount), and if the light was on or off (synchIsOn). Here is a pic of it during inPhase flashing!


One tip I have for past me is to comb through each line to figure out what is being done. I kept getting stuck as to why my code wasn't working and moving lines of code around was helpful when the light wasn't doing what I wanted it to. But at one point, it wouldn't stop being on, and Iris helped point me to where I forgot to update a variable.

I also finally learned how to print on Arduino after kind of ignoring it... but it was very helpful!! Especially since the lights flash for portions of a second and are hard to count. Even increasing the amount on the timing variables help us visually see what is happening.
