---
layout: page
title: Software
permalink: /software/
---

For a better look at our code, check out our [GitHub repository](https://github.com/hanyolo-shootsfirst/hanyolo).

Our two most important tasks were telling the robot how to move and sensing Ewoks. We decided to delegate each of theses tasks to a separate microprocessor: a [TINAH](https://projectlab.engphys.ubc.ca/enph253_2018/tinah-2018/) board (based off a wiring board) would control all aspects of the robot related to motion, and an Arduino would handle all tasks related to sensing and picking up Ewoks.

## TINAH

Originally, we divided the course into a series of states that corresponded to different actions. While elegant, this involved continuously checking to see what state we were in; instead, we opted to use a series of loops that didn't let our robot move on to another task until it had completed the current one.

<div style="text-align:center"><img style="width:70%" src="/assets/tinahflowchart.PNG"></div>

## Communication
To keep coordination between our microprocessors as simple as possible, we had three lines of communication. The TINAH output two "enable" signals for right and left that told the Arduino where and if it should be looking for Ewoks. The Arduino had one signal that told the TINAH to pause while the claw rescued an Ewok, and resume motion afterwards.

<div style="text-align:center"><img style="width:50%" src="/assets/comm.PNG"></div>

## Arduino

While our robot moved, the Arduino continuously looked for Ewoks. When one was found, it activated the claw. Through calibration, we determined the angles on our servo motors that corresponded to appropriate positions for the claw, and wrote functions such as `pickUpRight();` and `dropoff();`.

<div style="text-align:center"><img style="width:70%" src="/assets/arduinoflowchart.PNG"></div>

