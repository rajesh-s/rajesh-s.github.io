---
layout: post
date: 2026-06-27 15:59:00-0400
title:  isca26
inline: false
related_posts: false
---

Attended [ISCA '26](https://iscaconf.org/isca2026/) in Raleigh, NC, my first ISCA!

Takeaways:

- **Computer architecture is becoming system architecture.** The important design unit is no longer an isolated CPU, GPU, accelerator, memory, or network. The talks repeatedly optimized interactions across all of them, often extending down into packaging and cooling and up into compilers, runtimes, and application behavior.
- **Peak compute is no longer the most useful headline metric.** Capacity, data-movement efficiency, synchronization, tail latency, energy, reliability, and the ability to sustain utilization increasingly determine useful performance.
- **Specialization creates an orchestration problem.** Chiplets, DPUs, near-memory compute, dataflow engines, and heterogeneous memory tiers provide efficiency only when software can discover workload behavior and map each phase to the right resource without excessive movement or control overhead.
- **The memory hierarchy is becoming fluid.** HBM, LPDDR, CXL memory, flash, remote storage, and shared KV-cache services are turning placement into a dynamic system decision rather than a fixed hardware property.
- **Observability and programmability are architectural features.** Many promising mechanisms depended on exposing access patterns, phase behavior, locality, or communication intent while preserving simple interfaces for software. Hardware capability without a usable control and visibility model is insufficient.
- **Cross-layer co-design is becoming unavoidable.** Algorithmic changes such as sparsity, KV-cache approximation, and MoE routing interact directly with memory systems, collectives, topology, and packaging. Local optimization at one layer can easily move the bottleneck or increase total system cost elsewhere.
- **Simulation is essential because intuition does not scale to emerging systems.** Rack-scale AI machines, chiplet PHY behavior, disaggregated fabrics, and heterogeneous memory systems are expensive or unavailable, while their interactions are too nonlinear for fixed-latency or peak-bandwidth reasoning.
- **Deployability distinguishes an interesting idea from a useful system.** Several talks emphasized compatibility with existing software, repurposing available hardware mechanisms, avoiding critical-path changes, open representations, and sustained open-source maintenance.