---
layout: project
title: SLF Centrifugal Density Separator
description: A mechanical, non-chemical solution for removing Spotted Lanternfly (SLF) contamination from grape harvests.
image: /assets/images/Spotted_lanternfly.png
---

### Problem
Viticulturalists in New York State are affected by the spotted lantern fly infestation, an invasive species that contaminates the harvest. Batches are rejected from juiceries and wineries, resulting in economic loss. Traditional pest-control methods are insufficient. Pesticides come with high economic and environmental costs. Egg removal proves too difficult because of the massive scale of laying locations, costing too much in labor. 

### Impact
Reducing SLF contamination in harvest improves economic output. Currently, farmers rely on insecticide rotations, but a mechanical device would offer a low-chemical alternative and reduce the cost of expensive sprays while meeting the growing consumer demand. 

### The Solution: Centrifugal Density Separator
Our team proposed a high-speed rotation device that separates harvested grapes from SLF by density. This mechanical approach offers a low-chemical alternative to expensive sprays while meeting the growing consumer demand for organic integrity.

### Implementation
Harvest is loaded into the device, and an internal drum spins at a calculated RPM. Heavier grapes are pushed out furthest, sliding down the angled outer walls into a collection bin. Lighter insects get pulled into a secondary bag. This way, grape pulp is conserved without contamination. 

### Why It's Better than the Status Quo
Pesticides leave a taint on the wine’s taste profile and contaminate the organic integrity of the grapes. Manual sorting is slow, costly, and prone to human error/inconsistencies. Our solution is non-chemical and efficient on a large scale.

### End-of-Semester Proof-of-Concept
A benchtop rotating drum prototype using grapes and 3D printed SLF accurate to weight and size, allowing us to optimize RPM. Success is determined by comparing the percentage of pests (SLF models) successfully sorted with the percentage of harvest lost.

### Key Risks & Testing
To move from a concept to a viable product, we identified several key unknowns that require rigorous physical testing:

| Risk Factor | Engineering Concern | Mitigation/Testing |
|:---|:---|:---|
| **Grape Damage** | High RPM exerts force on the skin, potentially causing ruptures. | **Burst Test:** Spin grapes at incremental RPMs to find the failure point relative to separation speed. |
| **Mass Variation** | SLF density increases if they are soaked in juice or wedged in clusters. | **Obstruction Test:** Use 3D-printed, weighted SLF models to measure removal efficiency in dense clusters. |
| **Efficiency** | Centrifuges are batch processes; slow throughput may lead to farmer rejection. | **Time Trials:** Measure the cycle duration of the prototype to compare it against manual sorting speeds. |

---

### Client Questions
1. How much material other than grapes, like stems and leaves, typically remains in the bin after your primary harvest? This changes our separation threshold and testing parameters based on what we want to separate/how much grapes weigh.
2.What is the maximum holding time allowed between the grape being picked and it reaching the crusher before you worry about quality loss? This determines the constraints of our time trials and whether or not our product is viable in the time scale of grape processing.
3. Do the SLF tend to stay on the surface of the grape clusters when disturbed, or do they retreat deep into the center of the bunch? This affects the “ramping profile” (i.e. how fast we accelerate) based on how hard SLF tends to stay on grapes, and also how we simulate SLF in our separation experiments.
4. What reservations does this idea leave you with as a client? (Any issues we haven’t thought of?)


### References
* Penn State Extension: "Spotted Lanternfly Management in Vineyards."
* NYS Department of Environmental Conservation: "Spotted Lanternfly - NYDEC."