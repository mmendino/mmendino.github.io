---
layout: post
title: Update on the Knitting-Aid
subtitle: How the project is going >.<
author: Melissa Mendino Solano
tags: [final project, update]
---

A quick update on the coding portion of the Knitting-Aid project! It is going well I think!!
There has been many times already when I have been stuck and frustrated, but I'm having fun :)

Things that need to be coded:
- if I press the button
  - row count increases by 1
- if I reach 10 rows
  - the buzzer plays a short tune
  - RGB led turns on
  - RGB led stays on until I press the button
- if the light sensor receives light
  - the row count is separated into place values
  - 4 LEDs turn on to show row count in binary
  - a different color on the RGB light shows which place value

I began trying to create the counter, but because the code looped so quickly, one quick tap of the button created hundreds of rows.
I realized that I could create a state variable to help, and it didn't really work because it still created a ton of rows, but I knew it was needed.
Honestly, I saw that a delay helped, but I figured there was another way I could do it without it, but couldn't figure it out. Therefore, I added a short delay after the digital read of the button to only add one row. 
Wait I almost forgot, I tried to do an analogRead of the button value and found that 14 was the lowest, but changing the if statement to that didn't work either. 

I ended up choosing Tinkerbell's opening theme song on the DS game for the short tune!! I initally wanted to do a Mario Bros
coin sound but I didn't like how it was coming out. I found the sheet music for the Tinkerbell tune and had my fiancé, Vincent, help me read the music and figure out the beats per minute.
From there, I found a website that told me how to figure out the length of a quarter note for the BPM and the frequency for the different notes. 

Once I tried to add the music code to the if statement determining if the row%10=0, I ran into a few issues. The music kept looping and wouldn't allow for the button value to be updated because of the delays.
I tried to add a for statement in the music function, but it didn't work. I ended up putting it in the main loop void() function for the music function and that worked!
Having the RGB light turn cyan for the duration of being on the 10th row was pretty straight forward and I was able to do it!

Where I am stuck now is the part of the code where the 4 leds show the current row number and turn on a different rgb color based on the place value. I had to mess around with the scope of the variables determining the
number in the place value for the ones, tens and hundreds, but ended up placing them within the main void() function.
My code for this is working in a separate file, where I tested it. It turns on the binary number with red, blue or green depending on place value.
But for some reason the color stays blue for all place values in final file.

Things I've learned so far? How to kind of read music sheets! To experiment with your code if it doesn't do what you want.
To be super careful when moving code from different files because the variables were named differently :(. 
