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
Viticulturalists in New York State are facing a spotted lanternfly (SLF) infestation, an invasive species that contaminates grape harvests. Currently, batches are rejected by juiceries and wineries, causing significant economic loss. Traditional pest control, like heavy pesticide rotations, is environmentally costly and threatens organic integrity.

### Impact
Reducing SLF contamination in harvest improves economic output. Currently, farmers rely on insecticide rotations, but a mechanical device would offer a low-chemical alternative and reduce the cost of expensive sprays while meeting the growing consumer demand. 

### The Solution: Water-Based Agitation
Our team is developing a water-based agitation system that leverages **density-driven buoyancy** to separate SLF from grapes. Because grapes are denser than the invasive insects, controlled turbulence allows the SLF to float to the surface for removal while the grapes remain submerged.

### Implementation
Harvested fruit is loaded into a 3D-printed stationary bucket filled with water. A handheld drill powers a machined aluminum shaft connected to an agitator head. By oscillating the rotation, the system breaks the surface tension between the insects and the fruit.

### Why It's Better than the Status Quo
Pesticides leave a taint on the wine’s taste profile and contaminate the organic integrity of the grapes. Manual sorting is slow, costly, and prone to human error/inconsistencies. Our solution is non-chemical and efficient on a large scale.

### End-of-Semester Proof-of-Concept
Our project has pivoted to a water-based agitation system that utilizes density-driven buoyancy to separate invasive Spotted Lanternflies (SLF) from grape harvests. The system consists of a stationary 3D-printed bucket filled with water, where a machined aluminum shaft and a press-fit propeller create controlled turbulence. By oscillating the direction of agitation, we break the physical entanglements between the pests and the fruit. Success for the final design is defined by a separation efficiency of 90% of SLF models and a processing throughput of 4 minutes per 1kg batch.

### Key Risks & Testing
Through the development of our functional prototype, we identified and tested several critical mechanical risks to ensure the viability of the final product:

| Risk Factor | Engineering Concern | Mitigation/Testing & Results |
| :--- | :--- | :--- |
| **Agitation Effectiveness** | Single-direction spinning may not provide enough turbulence to free trapped insects. | **Directional Test:** Compared constant vs. oscillating rotation. Bi-directional agitation achieved a superior **84.5% separation rate**. We will automate direction switching using a programmable controller. |
| **Vortex Geometry** | Propellers that are too small may not create a sufficient "lift" zone for separation. | **Turbulence Test:** Measured vortex depth at varying power levels. Depth was insufficient at low RPM (4-5mm). We are **scaling the propeller diameter by 2.2x** to increase vortex width. |
| **Structural Fatigue** | High-resistance water agitation puts significant stress on 3D-printed joints. | **Cycling Test:** Operated the device for 20 cycles of 30 seconds. The socket developed **2.7mm of rotational play**. We will implement a secure mechanical lock/keyway for the final iteration. |
| **Containment & Seals** | Water loss through the shaft entry point could lead to messy operation or equipment damage. | **Leak Test:** Measured an average water loss of **0.35–0.7 ml/min**. We will integrate a professional-grade shaft seal from McMaster-Carr to ensure a watertight basin. |

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
This prototype was built to vet the mechanical design, specifically focusing on fabrication, assembly, and the effectiveness of bi-directional agitation.

**Core Components:**
* **Agitator Bucket:** A 3D-printed PLA vessel that acts as the stationary outer tank.
* **Machined Shaft:** An Al 6061 rod that transfers rotational motion from the drill to the agitator.
* **Agitator Head:** A press-fit PLA propeller designed to create water turbulence.

<div style="display:flex; gap:20px; justify-content:center; flex-wrap: wrap;">

<div style="text-align:center;">
  <img src="{{ site.baseurl }}/assets/images/shaft.png" width="250">
  <p><em>Shaft</em></p>
</div>

<div style="text-align:center;">
  <img src="{{ site.baseurl }}/assets/images/agitator_bucket.png" width="250">
  <p><em>Agitator Bucket</em></p>
</div>

<div style="text-align:center;">
  <img src="{{ site.baseurl }}/assets/images/agitator_bucket_shaft_connection.png" width="250">
  <p><em>Agitator Bucket and Shaft Connection</em></p>
</div>

</div>

### Assembly Instructions
**Step 1: Prepare the Shaft**  
Insert the machined aluminum shaft through the center hole of the agitator bucket. Ensure the flange sits flush against the rim to prevent vertical motion.
**Step 2: Attach the Agitator Head**  
Press-fit the agitator head onto the shaft inside the bucket. Confirm a tight fit with no rotational play.
**Step 3: Verify Clearance**  
Manually rotate the shaft to ensure the agitator spins freely without contacting the bucket walls.
**Step 4: Install Support Legs**  
Insert the 3D-printed legs into the base of the bucket. Ensure they are securely fitted.
**Step 5: Connect the Drill**  
Insert the shaft into the drill chuck and tighten. Verify bidirectional rotation capability.
**Step 6: Load the System**  
Fill the bucket to the marked water line. Add grape and SLF models.
**Step 7: Operate the Device**  
Run the drill, alternating direction every ~2 seconds to create oscillating agitation. Operate for 30–60 seconds.

### Performance Testing & Outcomes
We performed a series of design tests to identify mechanical risks and determine necessary iterations.

| Test | Objective | Result | Design Change Needed |
|:---|:---|:---|:---|
| **Agitation Method** | Compare single-direction vs. bi-directional spinning. | Bi-directional agitation achieved **84.5% separation**, showing less variance than single-direction. | Automate direction switching using a programmable motor controller instead of a manual drill trigger. |
| **Turbulence Range** | Determine if the propeller creates enough "lift". | Vortex depth was insufficient at low speeds (only 4–5mm at 25% power). | **Scale the propeller diameter by ~2.2X** to increase vortex width and depth. |
| **Structural Integrity** | Test the "Drill-to-Propeller" joint over 20 cycles. | The socket developed 2.7mm of rotational play/wear, though no cracking occurred. | Implement a more secure mechanical lock between the shaft and the agitator. |
| **Leakage** | Measure water loss through the shaft seal. | Average water loss ranged from **0.35 to 0.7 ml/minute**. | Improve 3D print tolerances and source a professional shaft seal from McMaster-Carr. |

### Success Criteria
To evaluate the final iteration, we have established the following quantitative targets:

1.  **Separation Efficiency (High Priority):** 90% of SLF models successfully separated after a 60-second cycle.
2.  **Processing Throughput (Medium Priority):** 4 minutes per 1kg batch, measured from "lid-touch to ready".
3.  **Operating Stability (Medium Priority):** Device movement 2 cm and water spillage 50 ml during maximum RPM operation.

### Exhibit Day Demonstration
We will demonstrate **Criterion 1** by processing a contaminated batch of 3D-printed grape and SLF models in real-time. After a 30-second agitation cycle, we will weigh the recovered SLF models on a scale to prove the 90% efficiency target has been met.