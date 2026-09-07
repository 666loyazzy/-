# Research Gaps and Testable Hypotheses — DynoPipe Direction

This file records **questions to test**, not established claims.

## G1. Decode-Critical WAN Dependence

**Hypothesis:** In single-boundary Edge→Cloud layer partitioning, autoregressive Decode may keep WAN transfer on the critical path for each generated token, making TPOT highly sensitive to RTT and jitter.

### Experiments
- Sweep RTT: 1 / 5 / 10 / 20 / 50 / 100 ms.
- Sweep bandwidth independently.
- Add jitter and packet loss.
- Compare TTFT, TPOT, P99, throughput, communication volume, and WAN interactions per token.
- Compare edge-only, cloud-only, static split, and dynamic split.

## G2. Prefill and Decode May Need Different Split Policies

**Hypothesis:** A split point that is good for Prefill may be poor for Decode because the two phases have different compute, memory, parallelism, and latency characteristics.

### Candidate experiment
Compare one unified split policy against phase-aware split-point selection while keeping the same edge-cloud architecture.

## G3. Communication Frequency vs Communication Volume

Current partition objectives often emphasize bytes transferred. Interactive LLM inference may also need to optimize:
- number of cross-domain transfers;
- synchronization frequency;
- serialization/deserialization events;
- RTT exposure per generated token.

## G4. Boundary Migration Cost

Dynamic split points are useful only if the cost of changing placement is lower than the expected benefit.

Questions:
- When should the system move a boundary?
- Which state must migrate?
- When is KV transfer better than recomputation?
- Can migration overlap with ongoing inference?
- How much hysteresis is required to avoid oscillation?

## G5. Weak-Network Robustness

A practical DynoPipe-style system should degrade gracefully under:
- bandwidth collapse;
- high RTT;
- jitter;
- packet loss;
- intermittent connectivity;
- cloud overload.

## G6. Realistic Edge Hardware Gap

**Question:** Do conclusions obtained on server-class edge GPUs hold on mobile / embedded / lower-memory platforms?

Candidate platforms:
- Jetson-class devices
- laptop GPUs
- integrated GPUs / NPUs where feasible

## G7. Mobility-Aware Placement

When the endpoint moves, bandwidth, RTT, and reachable edge resources can change together. Static or purely reactive split-point selection may lag behind these changes.

Questions:
- Should future resource state be predicted?
- How much benefit comes from proactive migration?
- Can endpoint mobility and boundary migration be optimized jointly?

## G8. Multi-Dimensional Objective

A practical controller may need to jointly optimize:
- TTFT
- TPOT
- P99 latency
- throughput
- edge memory
- communication volume
- migration overhead

A single throughput-oriented objective may not capture interactive edge workloads.

## Decision Rule

A gap becomes an experiment only when:
1. related DynoPipe-direction papers have been checked;
2. the issue is not already solved by prior work;
3. the hypothesis is measurable;
4. a realistic baseline and network setup exist.
