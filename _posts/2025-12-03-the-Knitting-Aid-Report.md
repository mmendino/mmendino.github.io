---
layout: post
title: the Knitting-Aid! Report
subtitle: Final Report of the creation of the Knitting-Aid
thumbnail-img: /assets/img/knittingAid_Comp.jpg
tags: [final project, complete]
author: Melissa Mendino Solano
---

<center><img src="/assets/img/knittingAid_Comp.jpg" width="80%" /></center>
<center>the Knitting-Aid!</center>

the Knitting-Aid! is an adorable teacup-shaped product helps a knitter (or crocheter) keep track of their rows and informs them when it is time to make a change! This specific model shows the knitter when they are on every 10th row to increase or decrease their stitches. You simply need to press the teabag shaped button after you have completed a row, and it will keep track of the total rows. When you reach the 10th row, a little tune will play and a cyan light will turn on!

The motivation for this product arose from my issue trying to keep track of my rows while knitting the Sophie Hood by PetiteKnit. I was knitting the large size where I had to increase every 10th row, but only had a notebook and pen to count my rows. I would lose my pen pretty often, which is why, with the Knitting-Aid, you simply have to push a button to count your rows and it will inform you when it is time to increase. *(Plus it's prettier than other row counters)*

When you have completed 9 rows, and on your 10th row, the RGB light on the Lilypad with turn cyan and the Tinkerbell DS Game Title Theme music will play. The tune only plays once, but the cyan light stay on until you complete the 10th row. It will do so for every 10th row and can go up to 999 rows.

To see what row number you are on, you simply open a flap to allow the light sensor to recieve light. The 4 pink LEDs will light up a number from 1-9 shown in binary code and 0 is represented by all of them on. The row count will be separated into place values. The RGB light on the Lilypad tells you whether the pink LEDs will show you the ones, tens, or hundreds place! The red is ones, green is tens, and blue is hundreds.

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
 4 pink LEDs | 1 sheet of pink felt | 1 sewing needle
 1 Buzzer | 1/5 light purple felt | scissors
1 spool of conductive thread | 1/5 dark purple felt | pack of alligator clips
1 Lilypad Arduino | 1/8 green felt | 1"x 2" velcro strip
1 Light Sensor | 1/4 white felt |
1"x 2" Conductive Fabric |1 pink embroidery floss |
1 LiPo Battery | 1 cream embroidery floss |
| |small bag polyfill stuffing |
| | 1 white embroidery floss |
| | 1 green embroidery floss|

### Prototyping Stages
#### Paper Prototype:
Front of the teacup
<p float="center">
<img src="/assets/img/theKnittingAid Front Prototype.jpg" width="90%" />
</p>
Back of the teacup
<p float="center">
<img src="/assets/img/theKnittingAid Back Prototype.jpg" width="90%" />
</p>

#### Lilypad Onboard LEDs and Button Prototype:


#### Alligator Clip Prototype:
<p float="center">
<img src="/assets/img/knittingAid_alligator.jpg" width="90%" />
</p>

<details markdown="1">
<summary>The Inside and Outside of my circuit</summary>
<center><img src="/assets/img/knittingAid_inside.jpg" width="80%" /></center>
<p>
</p>
<center><img src="/assets/img/knittingAid_outside.jpg" width="80%" /></center>
</details>

### Final Product
<p>
</p>
<center><b>Front and Back of the Knitting-Aid!</b></center>
<p float="center">
<img src="/assets/img/knittingAid_Comp_front.jpg" width="48%" />
<img src="/assets/img/knittingAid_Comp_back.jpg" width="48%" />
</p>
<p float="center">
<img src="/assets/img/knittingAid_Vid_outside.gif" width="70%" />
</p>


## The Knitting-Aid! in Action!
#### Adding 3 to the row count, and opening the light sensor flap to make the pink LEDs light up with the binary number.
<p float="center">
<img src="/assets/img/knittingAid_Vid_Counts.gif" width="70%" />
</p>

#### Reaching 9 completed rows to be working on the 10th row. Cyan light turns on and the Tinkerbell tune plays.
<p float="center">
<img src="/assets/img/knittingAid_Vid_buzzer_13.34.16.gif" width="70%" />
</p>

**Tips to my past self!**
- Do not forget to code your project in sections! I was overconfident and tried to code my actions all together, but realized that I couldn't test it unless it was in separate files.
- For the button counter, utilize two different state variables to determine if the button is pressed, and if it was previously pressed or not. Also a small delay will not completely kill your code!
- *analogRead* for the button doesn't work to make the counter.
- Carefully comb through the scope of the different functions created. I was having trouble with the colors that changed for the place values of the rowNumber, but it turned out that it was because one of my variables wasn't being seen by the function.
- Add a *for* statement to make sure that the buzzer only plays once!

**Proud of myself for:**
- Making the code easy to modify for different patterns! You simply need to update the changeRow at the top of the code and it will do the math for you!
- Getting the button to work!!
- Learning to read binary numbers
- Coding music from a music sheet
- using the onboard LEDs to test my code

Citations:
- Vincent helped me read the sheet music and figure out the note frequencies.
- Tinkerbell DS Game Title Theme: [musescore](https://musescore.com/user/84558067/scores/19627369)
- Turninig Music Sheet to Arduino Code: [Intructables](https://www.instructables.com/Arduino-Music-From-Sheet-Music/)
- .mov videos to .mp4: compress.mov
- .mp4 to .gif: Freeconvert.com
