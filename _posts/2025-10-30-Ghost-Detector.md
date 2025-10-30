---
layout: post
title: Ghost Detector
subtitle: Ghosts come out when it's dark and cold :(
tags: [light-sensor, temp-sensor, ghosts]
author: Melissa Mendino Solano
---

Sound the ghost alarm when it's dark and cold because the ghosties might sneak up on us! For this assignment, I had to turn on the onboard red LED and another red LED whenever it was cold and dark.

I began by figuring out the maximum and minimum values that the temperature and light sensors detected, then figured out where the dark and cold thresholds should be. For the temperature sensor, I converted the raw values into degrees farenheight to ensure it was working correctly and to understand how sensitive the sensor is.

With the thresholds, the red LEDs will turn on only if the light and the temperature and below the thresholds.

Here is an image of the LEDS turning on when the temperature is cold and I am blocking the light detector to make it dark.


Tip to past me: Convert the raw temperature values! It is easier to see how much you are affecting the temperature sensor if you understand the values. I held the temperature sensor between my fingers to make it warmer, but making it colder was harder when I was stuck in Schow.
