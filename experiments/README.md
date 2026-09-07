# Experiment Plan — DynoPipe Direction

Experiments have not started yet. This file defines the baseline protocol for **dynamic edge-cloud LLM partitioning/orchestration**.

## Stage 0 — Reproduce DynoPipe-Style Baselines
- Obtain code / artifacts for DynoPipe and the closest available dynamic split baselines.
- Reproduce at least one key table or figure before proposing a modification.
- Record software versions, model versions, hardware topology, and network configuration.

## Stage 1 — Network Sensitivity
Control bandwidth, RTT, jitter, and packet loss independently.

Suggested sweep:
- RTT: 1, 5, 10, 20, 50, 100 ms
- bandwidth: 100 Mbps, 500 Mbps, 1 Gbps, 5 Gbps, 10 Gbps
- optional jitter / loss after the basic sweep is stable

## Stage 2 — Prefill / Decode Breakdown
Measure separately:
- TTFT
- Prefill latency
- TPOT
- Decode tokens/s
- queueing
- cross-domain transfer volume
- cross-domain interactions per token

## Stage 3 — Split-Point / Boundary Study
Compare:
1. edge-only
2. cloud-only
3. static split
4. DynoPipe-style dynamic split
5. alternative dynamic split-point policies
6. phase-aware split policy if the baseline measurements justify it

## Stage 4 — Migration Cost
Measure:
- parameter/state movement
- KV-cache migration
- migration vs recomputation
- service interruption during reconfiguration
- benefit threshold required to justify a boundary move

## Stage 5 — Hardware and Mobility
When hardware is available:
- compare server-class edge GPU with more constrained devices;
- replay bandwidth/RTT traces representing 4G/5G/Wi-Fi or endpoint mobility.

## Reproducibility Checklist
- [ ] fixed model version
- [ ] fixed tokenizer
- [ ] fixed prompt set
- [ ] warmup policy documented
- [ ] batch/concurrency documented
- [ ] network shaping documented
- [ ] repeated runs with variance/error bars
- [ ] raw logs preserved
- [ ] scripts version-controlled

## Rule
Do not design the final method before baseline measurements establish that the target DynoPipe-style bottleneck exists.
