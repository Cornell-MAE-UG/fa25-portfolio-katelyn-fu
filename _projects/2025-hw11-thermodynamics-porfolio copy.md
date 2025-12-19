---
layout: project
title: HW 11 Heat Exchanger Lab
description: 
image: /assets/images/heat-exchanger.jpg
---

### Supplies: 
one heat exchanger, two water pumps, 4 water buckets, ice, water, styrofoam for insulation, an immersion heater, one thermocouple, four thermometers, food dye

### Description: 
A heat exchanger is a device that transfers thermal energy between two fluids at different temperatures without allowing the fluids to mix. In this system, heat is exchanged between hot and cold water streams flowing through separate channels inside the metal walls of the heat exchanger. The metal acts as a conductive barrier that allows energy to flow from the hotter fluid to the colder one while keeping the two fluids physically separated.

During operation, the hot water pumped from the heated reservoir enters one side of the heat exchanger and flows through its internal tubing, while cold water from the ice-cooled reservoir flows through a separate set of adjacent channels in the opposite direction. This counter-flow arrangement maintains a large temperature difference across the length of the device which enhances the rate of heat transfer and overall efficiency.

The driving mechanism of energy transfer is conduction through the metal wall and convection between the fluid and the surface. As energy moves from the hot to the cold stream, the hot water cools while the cold water warms. The process continues until the system reaches a quasi–steady-state condition where the inlet and outlet temperatures stabilize.

Heat exchangers like this are widely used in engineering and industrial applications where efficient heat recovery or dissipation is needed.

### System Diagram and Balances:  

<img src="/fa25-portfolio-katelyn-fu/assets/images/hw11-calculations.png"
     alt="Heat exchanger system diagram and balances"
     style="max-width: 100%; height: auto; display: block; margin: 0 auto;">

### Application of Energy Balance to Experimental Data:
Using the steady-flow energy balance derived above and assuming liquid water with constant specific heat (cp = 4.18 kJ/kg·K), the heat transfer rate can be calculated directly from measured temperatures. Kinetic and potential energy changes were assumed negligible, and no external heat loss to the surroundings was considered.
For the counter-flow case:

Q dot = m dot * cp (Th, in - Th, out)

Using a measured flow rate of 210 gal/hr (m dot = 0.22 kg/s):

Q dot = (0.22)(4.18)(35.0 - 18.6) = 15.0 kW

This result confirms quantitatively that counter-flow operation increases the heat transfer rate compared to same-flow operation under identical inlet conditions.
Because heat transfer occurs across a finite temperature difference, entropy generation is positive which confirms that real heat exchangers are irreversible devices. This entropy generation represents lost potential for useful work and provides a thermodynamic basis for improving exchanger design.

### Description of Change:
In our experiment, we compared the performance of the heat exchanger operating in same-flow (parallel-flow) and counter-flow configurations while keeping flow rate and inlet temperatures approximately constant. The main operating change was simply reversing one loop so the hot and cold streams flowed in opposite directions instead of the same direction.

### Measured Data

| Condition     | Th, in (°C) | Th, out (°C) | Tc, in (°C) | Tc, out (°C) |
|--------------|-------------|--------------|-------------|--------------|
| Same-flow    | 35.0        | 23.7         | 8.7         | 21.1         |
| Counter-flow | 35.0        | 18.6         | 9.2         | 22.1         |

Flow rate: **210 gal/hr** (constant for both trials)

In same-flow, the hot stream cooled by: 35.0 -23.7 = 11.3 °C
In counter-flow, the hot stream cooled by: 35.0 - 18.6 = 16.4 °C
Same-flow cold stream warmed by: 21.1 - 8.7 = 12.4 °C
Counter-flow cold stream warmed by: 22.1 - 9.2 = 12.9 °C
This indicates higher heat-transfer effectiveness in counter-flow.

In a parallel-flow configuration, the two fluids enter the heat exchanger at their largest temperature difference but rapidly approach one another, causing the driving temperature difference to decline along the length of the device. This limits the total amount of heat transfer, especially near the outlet.

In contrast, in counter-flow, the hot water entering at 35°C contacts cold water that is exiting (at ~22°C), while the hot outlet (18.6°C) contacts incoming cold at ~9°C. This maintains a larger temperature gradient over the entire device, which increases the heat transfer rate, the temperature change of both fluids, and the overall thermal effectiveness.



