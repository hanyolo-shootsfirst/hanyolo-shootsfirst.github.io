---
layout: page
title: Mechanical
permalink: /mechanical/
---

Our full robot CAD can be seen [here](https://cad.onshape.com/documents/b68df095191cfcbaff82ff1c/w/aba44803c1bc79aae08a4506/e/f46b62d9d5d4415f52d95b1e).

The mechanical components of our robot comprised five parts: the chassis, a basket, a scissor lift, two bridge(s) and a claw. We wanted to have a simple, modular design so that components could be tested separately and integrated later on. We used rapid prototyping techniques such as waterjet cutting, laser cutting, and 3D printing to manufacture our robot.   

![basketlift](/assets/basket_and_lift.jpg)

<p style="font-size:15px"  align="center"><em>The final chassis, all put together</em></p> 

## Chassis
<div style="text-align:center"><img style="width:50%" src="/assets/chassis.PNG"></div>

We made the chassis out of high density fiberboard (hardboard), a light, yet strong material with the laser cutter. We went through several iterations, and finally chose a design that had open sides that maximized accessibility for our circuitry, along with a dual-level system that would separate electrical components from moving mechanical components, such as the claw and scissor lift. 


## Claw

<table>
<tr><td style="width:50%;"><img style="width:70%;" src="/assets/clawcad.PNG"></td>
<td style="width:50%;"><img style="width:70%;" src="/assets/claw.jpg"></td></tr>
</table>

We wanted one central claw that could grab Ewoks from either side. To do this, we needed to be able to control the position of the claw, and so we elected to use a collection of servo motors. 

<div style="text-align:center">
<iframe src="//gifs.com/embed/claw-vo1R45" frameborder="0" scrolling="no" width="359px" height="416px" style="-webkit-backface-visibility: hidden;-webkit-transform: scale(1);"></iframe></div>

Initial prototypes were made from hardboard, which proved to be a bit too flimsy. We then tried polycarbonate, which was too heavy. Finally, we used the waterjet to cut aluminum sheet metal, with flanges for rigidity, and used two servos driven from the same signal pin to give us the torque we required to control the base.

##  Scissor Lift and Basket

<div style="text-align:center"><img style="width:50%" src="/assets/lift.png"></div>

We experimented with different materials for the scissor lift, but decided on acrylic for its lower friction (compared to hardboard) and lightness. After first looking into a rack and pinion system, then a spool and string mechanism, we settled on a lead screw system to actuate the lift, as this had the best balance of reliability, flexibility, and control.

The basket and scissor lift were designed together to work together. The Ewoks and Chewbacca occupied a lot of space, and to create that volume efficiently, we opted for a wide and short basket. 

## Bridge

Our bridge design followed our overall goal of keeping things simple. We added curled supports on the bottom of our bridge so that it would drop into the gap more reliably and be secure while we were moving across it.



