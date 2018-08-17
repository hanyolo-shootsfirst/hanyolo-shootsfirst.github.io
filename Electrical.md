---
layout: page
title: Electrical
permalink: /electrical/
---
<div style="text-align:center"><img style="width:100%" src="/assets/circuitry.jpg"></div>

To design an electrically robust system, we followed this framework:

1. Researching, prototyping and testing all circuits before integrating them into our system.
2. Minimizing the number of electrical components and substituting with software solutions where possible.
3. Applying safety measures such as:
    - adding decoupling capacitors in the right places
    - using shielded wire to minimize noise interference
    - making sure grounds are connected while avoiding ground loops
    - applying circuit buffers where necessary


For circuits which had a high likelihood of failure we made multiple sets of that circuit and designed our main PCB for easy exchange.

## Infrared signal circuit

![IR-circuit-diagram](/assets/ir_circuit.png)



R2D2 oscillated between emitting a 10 kHz and 1 kHz infrared wave. At 10 kHz, we were able to enter the Stormtrooper stronghold without triggering an alarm. This circuit was used to distinguish between these frequencies, and was particularly interesting because it was able to consistently detect and identify the signal from a distance of 10 meters!


## H-Bridge circuit

![H-Bridge Circuit](/assets/hbridge.png)
To enable differential drive, H-bridges were used to power motors. This H-Bridge circuit (developed by an ENPH alum Scott Lawson) was favourable because it was robust and easy to prototype onto a small PCB.
