---
layout: post
title: the Knitting-Aid! Proposal
subtitle: A plushie that helps you keep track of your knitting rows!
author: Melissa Mendino Solano
tags: [final project, proposal]
---

This is my project proposal for my final project:

**the Knitting-Aid! a companion to all knitters!**

I have been trying to knit the sophie hood by PetiteKnit this semester, hopefully to finish before I graduate. But I have been having a hard time keeping track of all of my rows. I need to increase and later decrease after every 10th row, but sometimes I forget to mark down what row I'm on, and get confused.
That's where the Knitting-Aid comes into play! It will keep track of my rows and all I have to do is press a button to let it know I have completed a row.
After every 10th row, the buzzer will play a little tune to congratulate me on my progress and a light will turn on to signal that it is time to do an increase.
The light will stay on until until I finish the row so that I don't forget that I am to do the increase in this row if it is at the end of the row.

There will also be an option to know what row I am one by opening a pouch to the light sensor, which will trigger the four leds on top to turn on depending on the number of row I am on in binary code.
I will also try to make it reset my rows by making it super bright.

Here is my proposal:
![project proposal slide for the Knitting-Aid! Includes motivation, what it does, and materials list](https://github.com/mmendino/mmendino.github.io/blob/master/assets/img/theKnittingAid3.0.jpg?raw=true)

Materials Available:
- 1 LilyPad Arduino Plus
- 1 light sensor
- 1 buzzer
- 4 pink LEDs
- green felt

Materials Needed:
- 2 1x1 inch pieces of conductive fabric
- 3 small Velcro dots (to store the tea bag on the back of the plushy and ensure the light sensor stays closed in)
- Felt sheets: ideally pink, purple, white, blue
- possibly fabric paint to insulate one of traces
- a small amount of stuffing so my plushy is soft

| Input | Output |
| :---: |:---: |
| Tea bag button | every 10th time, buzzer sounds and onboard RGB lights up cyan |
| Ambient light | 4 LEDs light up to show binary numbers |
| Bright light | Resets count|
| No Light | 4 LEDs are off|


