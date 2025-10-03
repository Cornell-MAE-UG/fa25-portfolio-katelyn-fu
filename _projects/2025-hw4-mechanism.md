---
layout: project
title: HW 4 Mechanism Design Portfolio Problem
description: Designing a lifting mechanism with a rigid bar, pin supports, and actuator
image: /assets/images/hw4_design.png
---


As part of a homework assignment, I designed a frame mechanism in a 2D space (150 cm x 50 cm) to maximize lifting height and weight capacity using a rigid bar, three pin supports, and a linear actuator.  

Design Choices:
- Bar length: 150 cm (rigid)  
- Actuator: Model IMA55 from https://www.tolomatic.com/wp-content/uploads/2022/05/2700-4000_29_IMA_cat.pdf (max force: 35.81 kN, stroke: 6.0 to 18.0 in, p1 = 1.9 in, BB = 11.49 in)  
- Pins: Two fixed at ground, one connecting actuator and bar  

How I solved the problem:
- Calculated the total length of the actuator by adding BB + stroke + P. I chose stroke to be 6 in because I wanted the actuator to start as short as possible. The IMA length was 19.39 in = 49.25 cm.
- Drew FBD of system including actuator, bar, and load
- Moment balance around point A to solve for F load which is the max load that my design can support.

Results: 
- Maximum lift height achieved: 50 cm
- Maximum load supported: 21.42 kN  

Final Design:  
![HW4 Mechanism Design](/assets/images/hw4_design.png)

