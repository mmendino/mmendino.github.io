---
layout: post
title: the Knitting-Aid, Update Two
subtitle: Code is up and running! Onto sewing!
tags: [final project, update]
author: Melissa Mendino Solano
---

This will be the last update on the Knitting-Aid until it is completed! I have worked out the bugs in my code and tested it with alligator clips with the layout of the physical product.
I have begun sewing my circuit on to the felt with my lilypad compenents and have it working it!

For the coding issue with the RGB colors showing the place value for the row count, it ended up being sort of a scope error! I had to move my segment of code
determining what color the RGB was to light up with the place value into the function for turning on the 4 LEDs showing the binary number.
Originally it worked in a separate file because my variables where within the main loop function, but since I created a new function for the code for the final project, it didn't see the variables I wanted it to see.

Another thing I changed was when the light would turn on the tune would play for the 10th row. I realized that it should turn on and play after I've completed the 9th row so that I know that I'm currently knitting the 10th row where I need to make the increase/decrease.

For the counter, I went over my code with Iris and realized that I did need a delay when I tried to make an alligator clip prototype. It had worked well withouht the delay with an extra state variable I had added, but once I unsnapped the lilypad components and created my alligator clip prototype, it was counting 2 or 3 for every button press.
I added the delay after this, and it worked well, so I left it at that.

The Knitting-Aid is officially in production now! I traced out my mug outline onto a sheet of pink felt and used tape to secure my lilypad compenents where I wanted them.
I have connected the buzzer, 4 LEDs, and light sensor! I need to finish sewing my button and connecting it to the lilypad then I can start some decorative stitching!
