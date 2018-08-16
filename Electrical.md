---
layout: page
title: Electrical
permalink: /electrical/
---

![circuitry](/assets/circuitry.jpg)

Our goal was to design an electrically robust system. How?

1. Researching, prototyping and testing all circuits before integrating them into our system.
2. Minimizing the number of electrical components and substituting with software solutions where possible.
3. Applying safety measures such as:
    - adding decoupling capacitors in the right places
    - using shielded wire to minimize noise interference
    - making sure grounds are connected while avoiding ground loops
    - applying circuit buffers where necessary


For circuits which had a high likelihood of failure we made multiple sets of that circuit and designed our main PCB for easy exchange.

# Some Key circuits

## Infra-Red signal Circuit

![IR-circuit-diagram](/assets/ir_circuit.png)
An infra-red signal detector circuit was used to distinguish between a 1kHz and a 10kHz signal being emitted by R2D2 to allow the robot into the Stormtrooper stronghold without triggering an alarm. This circuit was particularly interesting because it was able to consistently detect and identify the signal from a distance of 10 meters!


## H-Bridges

![H-Bridge Circuit](/assets/hbridge.png)
To enable differential drive, H-bridges where used to power motors. This H-Bridge circuit (developed by an ENPH alum Scott Lawson) was favourable because it was robust and easy to prototype on to a small PCB.
