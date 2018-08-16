---
layout: page
title: Software
permalink: /software/
---

Before we could write any code, we needed to figure when we needed to perform which tasks. Our two most important tasks were telling the robot how to move, and sensing Ewoks. We decided to relegate each of theses tasks to a separate microprocessor: a TINAH board (based off a wiring board) would control all aspects of the robot related to motion, and an arduino would handle all tasks related to sensing and picking up Ewoks.

##TINAH

Originally we structured we divided the course into a series of states, and the TINAH would perform different actions based on it's current state. While elegant, this involved continuously checking to see what state we were in; we opted to use a series of loops that didn't let our robot move on to another task until it had completed the current one.

[TINAH flow chart pic here]

##Arduino

While our robot moved, the Arduino continuously activated and read-in our Ewok sensors. When an Ewok was found, it activated the claw to pick up the Ewok. Through a lot of testing, we had already determined exacly what angles on our servo motors corresponded to a number of positions for the claw. Based on this, our code simply told the claw to go to a predetermined position for pick-up, drop-off, and travel.

[Arduino flow chart pic here]

##Communication
To keep coordination between our microprocessors as simple as possible, we had three lines of communication. The TINAH output two enable signals that told the Arduino where and if it should be looking for Ewoks. And the Arduino had a one signal that told the TINAH to pause all motion while the claw rescued an Ewok and then resume motion afterwards.

[communication pic here]