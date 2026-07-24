---
layout: post
date: 2026-06-27 15:59:00-0400
title:  Attended ISCA '26 in Raleigh, NC, my first ISCA!
inline: false
related_posts: false
---

Grateful to have met three generations of advisors today at the International Symposium on Computer Architecture (ISCA) in Raleigh, NC : Prof. Matt Sinclair, Prof. Sarita Adve, and Prof. Mark Hill.

It was a surreal moment to meet people whose decades of papers, books, and ideas have shaped how I think about parallel computer architecture and cache coherence. Their collective contributions, along with the mentorship of Prof. Sinclair, have set a remarkable example for me and continue to inspire my research in heterogeneous systems. 

Moments like this make me especially proud to be a Badger and to have been a part of the HAL research group. It was also a meaningful opportunity to connect with my broader academic family, including members of Prof. Adve’s group from UIUC and Prof. Sinclair’s group from Wisconsin.

<style>
.square {
  aspect-ratio: 1 / 1;     /* keep square automatically */
  width: 100%;             /* responsive */
  overflow: hidden;        /* hide cropped overflow */
  display: flex;
  align-items: center;
  justify-content: center;
}

.square img {
  width: 100%;
  height: 100%;
  object-fit: cover;       /* crop to square */
}
</style>

<div class="row mt-3">
  <div class="col-sm mt-3 mt-md-0">
    <div class="square">
      {% include figure.liquid loading="eager" path="assets/img/isca.jpg" class="img-fluid rounded z-depth-1" %}
    </div>
  </div>
</div>


Takeaways from the confernece:

- **Computer architecture is becoming system architecture.** The important design unit is no longer an isolated CPU, GPU, accelerator, memory, or network. The talks repeatedly optimized interactions across all of them, often extending down into packaging and cooling and up into compilers, runtimes, and application behavior.
- **Peak compute is no longer the most useful headline metric.** Capacity, data-movement efficiency, synchronization, tail latency, energy, reliability, and the ability to sustain utilization increasingly determine useful performance.
- **Specialization creates an orchestration problem.** Chiplets, DPUs, near-memory compute, dataflow engines, and heterogeneous memory tiers provide efficiency only when software can discover workload behavior and map each phase to the right resource without excessive movement or control overhead.
- **The memory hierarchy is becoming fluid.** HBM, LPDDR, CXL memory, flash, remote storage, and shared KV-cache services are turning placement into a dynamic system decision rather than a fixed hardware property.
- **Observability and programmability are architectural features.** Many promising mechanisms depended on exposing access patterns, phase behavior, locality, or communication intent while preserving simple interfaces for software. Hardware capability without a usable control and visibility model is insufficient.
- **Cross-layer co-design is becoming unavoidable.** Algorithmic changes such as sparsity, KV-cache approximation, and MoE routing interact directly with memory systems, collectives, topology, and packaging. Local optimization at one layer can easily move the bottleneck or increase total system cost elsewhere.
- **Simulation is essential because intuition does not scale to emerging systems.** Rack-scale AI machines, chiplet PHY behavior, disaggregated fabrics, and heterogeneous memory systems are expensive or unavailable, while their interactions are too nonlinear for fixed-latency or peak-bandwidth reasoning.
- **Deployability distinguishes an interesting idea from a useful system.** Several talks emphasized compatibility with existing software, repurposing available hardware mechanisms, avoiding critical-path changes, open representations, and sustained open-source maintenance.