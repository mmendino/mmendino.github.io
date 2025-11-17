---
layout: post
title: Analog Arrays
subtitle: Randomly turning on or off analog pins to a random value!
author: Melissa Mendino Solano
tags: [randoms, arrays, pwms, for loops]
---

For this assignment, we had to use the PWM (analog) pins on our Lilypad Arduinos! Every second the arduino has to choose a random pin and either turn it on to a random brightness or turn it if off if it was already on. I used an array to store the pin numbers, and also a boolean array to store whether the pin the was on or off. For the set up, I was able to use a for loop to set up the different pin numbers since they were in an array instead of having to set up each one individually. After that, I needed to choose a random pin, then a random brightness if the pin was off.

Here is a picture of when all of my PWM pins were randomly on, and another picture while the code was running.
![all the PWM lights are on](https://github.com/mmendino/mmendino.github.io/blob/master/assets/img/arrays1.jpg?raw=true)

![only the red, green and yellow lights are on](https://github.com/mmendino/mmendino.github.io/blob/master/assets/img/arrays2.jpg?raw=true)

Tip to myself: After the code works, go back to see what could be more efficient! I write out comments for what states I have to catch, and it helps me organize my code and write it out. But, I ended up using if, else if, instead of just if and else because I was writing what needed to happen. I simplified that, and then I realized that I had created an extra variable that I didn't need for the random pin choice, and was able edit my code further.
