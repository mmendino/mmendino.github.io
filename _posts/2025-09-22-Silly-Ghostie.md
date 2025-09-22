---
layout: post
title: Silly Ghostie
subtitle: Silly little ghost ASCII art!
tags: [cute, extra-credit]
author: Melissa Mendino Solano
---

As my first attempt at ASCII art, I have created a code to make a silly little lopsided ghost that tries to scare you by saying:
"i'm a ghostie ooooooooo"

I chose this because I am quite fond of little lopsided, flat ghosts with uneven eyes! My love of this ghostie comes from
the first time I tried applique - I attempted to applique a ghost but he ended up flat, spreading to the right, and with uneven eyes.

![A ghost made up of symbols saying i'm a ghostie](https://github.com/mmendino/mmendino.github.io/blob/master/assets/img/imaghostie.jpg?raw=true)

My ghostie is created by space characters, back slashes, forward slashes, dashes, underscores, astericks and letters.
A trick I learned is that to printf a backslash you need to type two backslashes.

If you would like to recreate this ghostie, or make it your own, you can find the code below!

```c
// A program to create a little lopsided ghost image that says i'm a ghostie

#include <stdio.h>
int main()
{

    printf("    *                *            *\n");
    printf("                   _______   *              *\n");
    printf("          *     _/        \\_    *      _____________\n");
    printf("      *        /   ^    ^    \\*       / i'm a       \\ \n");
    printf("   *          /    o    O      \\     <    ghostie    |\n");
    printf("             /   _         _     \\_  *\\ oOOOOOOooooo /\n");
    printf("         * _/         U            \\__ \\____________/   * \n");
    printf("   *      /                           \\ \n");
    printf("         /                              \\__   * \n");
    printf(" *    _/                                   \\_    *    \n");
    printf("     /                    _          ___      \\       *  \n");
    printf("    (______-----________--  -_______-   -- ____) \n");
    
    return 0;
}
```
