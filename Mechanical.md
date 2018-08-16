---
layout: page
title: Mechanical
permalink: /mechanical/
---

The mechanical components of our robot consisted of five main parts:

- chassis
- basket
- scissor lift
- bridge(s)
- claw

The philosophy we followed when designing each part of the robot was to have a simple modular design that we can test separately and easily integrate later.

We designed each component using [Onshape](https://www.onshape.com/), a free online CAD software, making collaboration a simple process. We manufactured our robot with a combination of laser cut, waterjet cut, and 3D printed parts.   

## Chassis

![chassisCAD](/assets/chassis.PNG)

We made the chassis out of high density fiberboard (hardboard), as it is a light, yet strong material easy to prototype on the laser cutter. We went through several iterations, tweaking it each time to accommodate other parts of our robot. We settled for a design that had open sides that maximized accessibility for our circuitry, along with a dual-level system that would separate electrical components from moving mechanical components, such as the claw and scissor lift. 

![final chassis with Ewok](/assets/Chassis_4.JPG)

## Claw

![claw](/assets/claw.jpg)
We wanted one central claw that could grab Ewoks from either side. To do this, we needed a high level of control in terms of the position of the claw, and so we elected to use a collection of servo motors. 

Initial prototypes were made from hardboard, which proved to be a bit too flimsy. We then tried polycarbonate, which was too heavy of a load for the servos. We thought about using a DC motor with touch sensors at a few key positions, but would add much more complexity to the design. Finally, we use the waterjet to cut aluminum sheet metal, with flanges for rigidity, and used two servos driven from the same signal pin to control the base, which required the most torque.
![CAD of claw](/assets/clawcad.PNG)

The full range of motion was a combination of

- 360 degree rotation about the base from a lazy susan bearing 
- 90 degree rotation at the base 
- 90 degree rotation at the "elbow" 
- Opening and closing of the grippers

<p style="text-align:center"><img src="/assets/clawgif.gif"></p>

##  Scissor Lift and Basket

![lift](/assets/lift.png)

We experimented with different materials for the scissor lift, but decided on acrylic for its lower friction (compared to hardboard) and lightness. After first looking into a rack and pinion system, then a spool and string mechanism, we settled on a lead screw system, as this had the best balance of reliability, flexibility, and control to actuate the lift.

![basket](/assets/basket.jpg)

The basket and scissor lift were designed together to work together. The Ewoks and Chewbacca occupied a lot of space, and to create that volume efficiently, we opted for a wide and short basket. 

## Bridge

![bridge](/assets/bridge.jpg)

Initially, we had ideas of lifting ourselves over the gaps with using two unfolding arms each in the front and back. Halfway into the design process we realized that this idea would take more time to implement than was given for this project. We then decided to use bridges to cross the gaps.

Our bridge design followed our overall motive of keeping things simple and easy to design. We used sheet metal as it is light but strong. We added curled supports on the bottom of our bridge so that it would drop into the gap more reliably and be secure while we were moving across it.

![basketlift](/assets/basket_and_lift.jpg)
