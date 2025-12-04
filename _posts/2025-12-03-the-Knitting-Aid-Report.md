---
layout: post
title: the Knitting-Aid! Report
subtitle: Final Report of the creation of the Knitting-Aid
tags: [final project, complete]
author: Melissa Mendino Solano
---

the Knitting-Aid! is an adorable teacup-shaped product helps a knitter (or crocheter) keep track of their rows and informs them when it is time to make a change! This specific model shows the knitter when they are on every 10th row to increase or decrease their stitches. You simply need to press the teabag shaped button after you have completed a row, and it will keep track of the total rows. When you reach the 10th row, a little tune will play and a cyan light will turn on!

The motivation for this product arose from my issue trying to keep track of my rows while knitting the Sophie Hood by PetiteKnit. I was knitting the large size where I had to increase every 10th row, but needed to keep a notebook and pen to count my rows. This wasn't very comfortable and sometimes I would lose my writing instrument, which is why, with the Knitting-Aid, you simply have to push a button to count your rows and it will inform you when it is time to increase.

When you reach every 10th row by pressing your completed 9th row, the RGB light with turn cyan and the Tinkerbell DS Game Title Theme music plays. The tune only plays once, but the cyan light will be on until you complete the 10th row.

To see what row number you are on, you simply open a flap to allow the light sensor to recieve light. The 4 pink LEDs will light up a number from 1-9 shown in binary code and 0 is represented by all of them on. The row count will be separated into place values. The RGB light on the lilypad tells you whether the pink LEDs will show you the ones, tens, or hundreds place! The red is ones, green is tens, and blue is hundreds.

Lights that will turn on depending of row count:

| Row Number | RGB color | Pink LEDs State |
| :---: | :---: | :---: |
3 | Red | OFF, OFF, ON, ON
25 | Green | OFF, OFF, ON, OFF
| | Red | OFF, ON, OFF, ON
342 | Blue | OFF, OFF, ON, ON
| | Green | OFF, ON, OFF, OFF
| | Red | OFF, OFF, ON, OFF


Materials List:

| Lilypad Components | Plushy Creation | Other |
| :---: | :---: | :---: |
 4 pink LEDs | pink felt | sewing needle
 Buzzer | light purple felt | scissors
conductive thread | dark purple felt | alligator clips
 Lilypad Arduino | green felt | velcro strip
 Light Sensor | pink thread |
Conductive Fabric | white felt |
 LiPo Battery | cream thread |
| | polyfill stuffing |

Here is an image of my alligator prototyping stage!
![Lilypad connected to many alligator clips and all the components needed](https://github.com/mmendino/mmendino.github.io/blob/master/assets/img/knittingAid_alligator.jpg?raw=true)

<details markdown="1">
<summary>The Inside and Outside of my circuit</summary>
<center><img src="/assets/img/knittingAid_inside.jpg" width="60%" /></center>

 
<center><img src="/assets/img/knittingAid_outside.jpg" width="60%" /></center>
</details>

<center><b>The Completed Knitting-Aid!</b></center>
![front of knitting-aid with teabag](https://github.com/mmendino/mmendino.github.io/blob/master/assets/img/knittingAid_Comp.jpg?raw=true)

<p float="center">
  <img src="assets/img/knittingAid_Comp_front.jpg" width="49%" />
  <img src="assets/img/knittingAid_Comp_back.jpg" width="49%" />
</p>

**Tips to my past self!**
- Do not forget to code your project in sections! I was overconfident and tried to code my actions all together, but realized that I couldn't test it unless it was in separate files.
- For the button counter, utilize two different state variables to determine if the button is pressed, and if it was previously pressed or not. Also a small delay will not completely kill your code!
- analogRead for the button doesn't work to make the counter.
- Carefully comb through the scope of the different functions created. I was having trouble with the colors that changed for the place values of the rowNumber, but it turned out that it was because one of my variables wasn't being seen by the function.
- Add a for statement to make sure that the buzzer only plays once!

**Proud of myself for:**
- Making the code easy to modify for different patterns! You simply need to update the changeRow at the top of the code and it will do the math for you!
- Getting the button to work!!
- Learning to read binary numbers
- Coding music from a music sheet
- using the onboard LEDs to test my code


Citations:
- Tinkerbell DS Game Title Theme: [musescore](https://musescore.com/user/84558067/scores/19627369)
- Turninig Music Sheet to Arduino Code: [Intructables](https://www.instructables.com/Arduino-Music-From-Sheet-Music/)
