---
layout: page
title: Software
permalink: /software/
---

For a better look at our code, check out our [GitHub repository](https://github.com/hanyolo-shootsfirst/hanyolo).

Our two most important tasks were telling the robot how to move and sensing Ewoks. We decided to delegate each of theses tasks to a separate microprocessor: a [TINAH](https://projectlab.engphys.ubc.ca/enph253_2018/tinah-2018/) board (based off a wiring board) would control all aspects of the robot related to motion, and an Arduino would handle all tasks related to sensing and picking up Ewoks.

## TINAH

The TINAH was our main processing unit, which controlled the motion of the robot. We used C++ and its object-oriented capabilities. Our code was arranged into a series of loops that didn’t allow our robot to move on to another task until it had completed the current one. 

<div style="text-align:center"><img style="width:70%" src="/assets/tinahflowchart.png"></div>

## Communication
We had three lines of digital communication. The TINAH output two "enable" signals for right and left that told the Arduino where and if it should be looking for Ewoks. The Arduino output one signal that told the TINAH to pause while the claw rescued an Ewok, and resume motion afterwards.

<div style="text-align:center"><img style="width:50%" src="/assets/comm.png"></div>

## Arduino

While our robot moved, the Arduino continuously looked for Ewoks. When one was found, it activated the claw. We wrote functions that would allow the claw to pick up on either side by writing appropriate angles to each servo motor.  

<div style="text-align:center"><img style="width:70%" src="/assets/arduinoflowchart.png"></div>

