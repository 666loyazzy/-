# Research Gaps and Testable Hypotheses

This file records **questions to test**, not claims to present as established facts.

## G1. Decode-Critical WAN Dependence

**Hypothesis:** In single-boundary Edge→Cloud layer partitioning, autoregressive Decode may keep WAN transfer on the critical path for each generated token, making performance highly sensitive to RTT and jitter.

### Why it matters
Optimizing transferred bytes alone may be insufficient if the number and timing of WAN interactions dominate TPOT.

### Experiments
- Sweep RTT: 1 / 5 / 10 / 20 / 50 / 100 ms.
- Sweep bandwidth independently.
- Add jitter and packet loss.
- Compare TTFT, TPOT, P99, throughput, and WAN interactions per token.
- Compare static split, dynamic split, edge-only, cloud-only, and phase-aware alternatives.

## G2. Prefill and Decode May Need Different Placement

**Hypothesis:** A placement that is good for Prefill may be poor for Decode because the two phases have different compute, memory, parallelism, and latency characteristics.

### Candidate direction
Phase-aware scheduling:
- Prefill: edge-cloud collaboration or cloud-heavy execution.
- Decode: edge-local or selectively cloud-assisted execution.

## G3. Realistic Edge Hardware Gap

**Question:** Do conclusions obtained on server-class edge GPUs hold on mobile/embedded platforms?

### Candidate platforms
- Jetson-class devices
- laptop/mobile GPUs
- NPUs
- integrated GPUs

## G4. Communication Frequency vs Communication Volume

Most placement objectives focus strongly on bytes transferred. A latency-sensitive interactive LLM may also need to minimize:

- number of cross-domain round trips;
- synchronization frequency;
- serialization/deserialization events;
- state migration frequency.

## G5. Weak-Network Robustness

A practical edge system should degrade gracefully under:
- bandwidth collapse;
- high RTT;
- jitter;
- intermittent connectivity;
- cloud overload.

Potential metric: quality/latency under a network-availability envelope, not only a fixed benchmark link.

## G6. Edge SLM + Cloud LLM Collaboration

Instead of layer-splitting one LLM, use:
- small local model for immediate generation;
- cloud model for verification/correction/planning;
- adaptive escalation only when needed.

This may reduce WAN dependence while preserving access to a stronger cloud model.

## G7. KV-Cache Placement and Migration

Questions:
- Which KV state should remain local?
- When is migration more expensive than recomputation?
- Can Decode-local KV state reduce cross-domain dependence?
- How does long context change the optimal strategy?

## Decision Rule

A gap graduates into an experiment only when:
1. at least several related papers have been checked;
2. the gap is not already solved by prior work;
3. there is a measurable hypothesis;
4. there is a realistic baseline and evaluation plan.
