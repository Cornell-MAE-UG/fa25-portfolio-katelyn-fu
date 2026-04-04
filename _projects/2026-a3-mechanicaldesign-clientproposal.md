---
layout: project
title: SLF Centrifugal Density Separator
description: A mechanical, non-chemical solution for removing Spotted Lanternfly (SLF) contamination from grape harvests.
image: /assets/images/Spotted_lanternfly.png
---

## Table of Contents
* [Client Pitch](#client-pitch)
* [Functional Prototype](#functional-prototype)

---

<a name="client-pitch"></a>
## Client Pitch

### Problem
[cite_start]Viticulturalists in New York State are facing a spotted lanternfly (SLF) infestation, an invasive species that contaminates grape harvests[cite: 447]. [cite_start]Currently, batches are rejected by juiceries and wineries, causing significant economic loss[cite: 447]. Traditional pest control, like heavy pesticide rotations, is environmentally costly and threatens organic integrity.

### Impact
Reducing SLF contamination in harvest improves economic output. Currently, farmers rely on insecticide rotations, but a mechanical device would offer a low-chemical alternative and reduce the cost of expensive sprays while meeting the growing consumer demand. 

### The Solution: Water-Based Agitation
[cite_start]Our team is developing a water-based agitation system that leverages **density-driven buoyancy** to separate SLF from grapes[cite: 447]. [cite_start]Because grapes are denser than the invasive insects, controlled turbulence allows the SLF to float to the surface for removal while the grapes remain submerged[cite: 447, 472].

### Implementation
[cite_start]Harvested fruit is loaded into a 3D-printed stationary bucket filled with water[cite: 467, 508]. [cite_start]A handheld drill powers a machined aluminum shaft connected to an agitator head[cite: 466, 468, 506]. [cite_start]By oscillating the rotation, the system breaks the surface tension between the insects and the fruit[cite: 507, 510].

### Why It's Better than the Status Quo
Pesticides leave a taint on the wine’s taste profile and contaminate the organic integrity of the grapes. Manual sorting is slow, costly, and prone to human error/inconsistencies. Our solution is non-chemical and efficient on a large scale.

### End-of-Semester Proof-of-Concept
[cite_start]Our project has pivoted to a water-based agitation system that utilizes density-driven buoyancy to separate invasive Spotted Lanternflies (SLF) from grape harvests[cite: 191, 210]. [cite_start]The system consists of a stationary 3D-printed bucket filled with water, where a machined aluminum shaft and a press-fit propeller create controlled turbulence[cite: 211, 212, 215]. [cite_start]By oscillating the direction of agitation, we break the physical entanglements between the pests and the fruit[cite: 131, 216]. [cite_start]Success for the final design is defined by a separation efficiency of $\ge90\%$ of SLF models and a processing throughput of $\le4$ minutes per 1kg batch[cite: 194, 197].

### Key Risks & Testing
[cite_start]Through the development of our functional prototype, we identified and tested several critical mechanical risks to ensure the viability of the final product[cite: 46, 110]:

| Risk Factor | Engineering Concern | Mitigation/Testing & Results |
| :--- | :--- | :--- |
| **Agitation Effectiveness** | [cite_start]Single-direction spinning may not provide enough turbulence to free trapped insects[cite: 127]. | [cite_start]**Directional Test:** Compared constant vs. oscillating rotation[cite: 123]. [cite_start]Bi-directional agitation achieved a superior **84.5% separation rate**[cite: 141]. [cite_start]We will automate direction switching using a programmable controller[cite: 143]. |
| **Vortex Geometry** | [cite_start]Propellers that are too small may not create a sufficient "lift" zone for separation[cite: 147]. | [cite_start]**Turbulence Test:** Measured vortex depth at varying power levels[cite: 148, 149]. [cite_start]Depth was insufficient at low RPM (4-5mm)[cite: 157]. [cite_start]We are **scaling the propeller diameter by 2.2x** to increase vortex width[cite: 161, 162]. |
| **Structural Fatigue** | [cite_start]High-resistance water agitation puts significant stress on 3D-printed joints[cite: 166]. | [cite_start]**Cycling Test:** Operated the device for 20 cycles of 30 seconds[cite: 168]. [cite_start]The socket developed **2.7mm of rotational play**[cite: 176]. [cite_start]We will implement a secure mechanical lock/keyway for the final iteration[cite: 177]. |
| **Containment & Seals** | [cite_start]Water loss through the shaft entry point could lead to messy operation or equipment damage[cite: 179, 181]. | [cite_start]**Leak Test:** Measured an average water loss of **0.35–0.7 ml/min**[cite: 188]. [cite_start]We will integrate a professional-grade shaft seal from McMaster-Carr to ensure a watertight basin[cite: 189]. |

---

### Client Questions
1. How much material other than grapes, like stems and leaves, typically remains in the bin after your primary harvest? This changes our separation threshold and testing parameters based on what we want to separate/how much grapes weigh.
2. What is the maximum holding time allowed between the grape being picked and it reaching the crusher before you worry about quality loss? This determines the constraints of our time trials and whether or not our product is viable in the time scale of grape processing.
3. Do the SLF tend to stay on the surface of the grape clusters when disturbed, or do they retreat deep into the center of the bunch? This affects the “ramping profile” (i.e. how fast we accelerate) based on how hard SLF tends to stay on grapes, and also how we simulate SLF in our separation experiments.
4. What reservations does this idea leave you with as a client? (Any issues we haven’t thought of?)


### References
* Penn State Extension: "Spotted Lanternfly Management in Vineyards."
* NYS Department of Environmental Conservation: "Spotted Lanternfly - NYDEC."


<a name="functional-prototype"></a>
## Functional Prototype

### Purpose & Design Intent
[cite_start]This prototype was built to vet the mechanical design, specifically focusing on fabrication, assembly, and the effectiveness of bi-directional agitation[cite: 273, 379].

**Core Components:**
* [cite_start]**Agitator Bucket:** A 3D-printed PLA vessel that acts as the stationary outer tank[cite: 464, 467].
* [cite_start]**Machined Shaft:** An Al 6061 rod that transfers rotational motion from the drill to the agitator[cite: 464, 468].
* [cite_start]**Agitator Head:** A press-fit PLA propeller designed to create water turbulence[cite: 464, 471, 500].

### Performance Testing & Outcomes
[cite_start]We performed a series of design tests to identify mechanical risks and determine necessary iterations[cite: 274, 302].

| Test | Objective | Result | Design Change Needed |
|:---|:---|:---|:---|
| **Agitation Method** | [cite_start]Compare single-direction vs. bi-directional spinning[cite: 383]. | [cite_start]Bi-directional agitation achieved **84.5% separation**, showing less variance than single-direction[cite: 393, 397]. | [cite_start]Automate direction switching using a programmable motor controller instead of a manual drill trigger[cite: 399]. |
| **Turbulence Range** | [cite_start]Determine if the propeller creates enough "lift"[cite: 403]. | [cite_start]Vortex depth was insufficient at low speeds (only 4–5mm at 25% power)[cite: 413]. | [cite_start]**Scale the propeller diameter by ~2.2X** to increase vortex width and depth[cite: 417, 418]. |
| **Structural Integrity** | [cite_start]Test the "Drill-to-Propeller" joint over 20 cycles[cite: 420, 424]. | [cite_start]The socket developed 2.7mm of rotational play/wear, though no cracking occurred[cite: 427, 432]. | [cite_start]Implement a more secure mechanical lock between the shaft and the agitator[cite: 433]. |
| **Leakage** | [cite_start]Measure water loss through the shaft seal[cite: 434, 437]. | [cite_start]Average water loss ranged from **0.35 to 0.7 ml/minute**[cite: 444]. | [cite_start]Improve 3D print tolerances and source a professional shaft seal from McMaster-Carr[cite: 445]. |

### Success Criteria
[cite_start]To evaluate the final iteration, we have established the following quantitative targets[cite: 304, 305]:

1.  [cite_start]**Separation Efficiency (High Priority):** $\ge90\%$ of SLF models successfully separated after a 60-second cycle[cite: 450].
2.  [cite_start]**Processing Throughput (Medium Priority):** $\le4$ minutes per 1kg batch, measured from "lid-touch to ready"[cite: 453].
3.  [cite_start]**Operating Stability (Medium Priority):** Device movement $\le2$cm and water spillage $\le50$ml during maximum RPM operation[cite: 455].

### Exhibit Day Demonstration
[cite_start]We will demonstrate **Criterion 1** by processing a contaminated batch of 3D-printed grape and SLF models in real-time[cite: 456, 457]. [cite_start]After a 30-second agitation cycle, we will weigh the recovered SLF models on a scale to prove the $\ge90\%$ efficiency target has been met[cite: 457].