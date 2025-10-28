---
layout: post
title: Button + Colors
subtitle: Button turns on an RGB light random colors!
tags: [buttons, randoms, state-base, RGB]
author: Melissa Mendino Solano
---

For this assignment, I had to write an Arduino program to turn on the onboard RGB light to a random color whenever the button was pressed. We learned how to include a button into our program, which was weird because LOW means it is pressed? And we learned how RGB lights make different colors and can be programmed to make whatever color you want!

I started by figuring out how to make the light turn on while the button was pressed and turn off when it wasn't pressed. After that I had to make sure that only one color was shown while the button was pressed, and I went a little further by limiting it to 12 colors. However, I couldn't figure out how to prevent it from randomly choosing all zeros, so sometimes the light donesn't turn on when the button is pressed because the Red, Green, and Blue lights are at zero.

Here is a picture of a random color turning on while I press the button!
![The button is being pressed and the light is on](https://github.com/mmendino/mmendino.github.io/blob/master/assets/img/randomcolors.jpg?raw=true)

One tip! My light would cycle through so many random numbers every time I pressed the button and I could not figure out how to catch the first random number. I realized I needed to make a state-based variable to help catch it and was able to figure it out from there.
