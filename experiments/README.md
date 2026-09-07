# Experiment Plan

Experiments have not started yet. This file defines the baseline protocol for when implementation begins.

## Stage 0 — Reproduce
- Obtain code / artifacts for representative systems.
- Reproduce one key table or figure before modifying anything.
- Record software versions and hardware topology.

## Stage 1 — Network Sensitivity
Control bandwidth, RTT, jitter, and packet loss independently.

Suggested sweep:
- RTT: 1, 5, 10, 20, 50, 100 ms
- bandwidth: 100 Mbps, 500 Mbps, 1 Gbps, 5 Gbps, 10 Gbps
- optional jitter / loss after the basic sweep is stable

## Stage 2 — Phase Breakdown
Measure Prefill and Decode separately:
- TTFT
- Prefill latency
- TPOT
- decode tokens/s
- queueing
- cross-domain transfer volume
- cross-domain interactions per token

## Stage 3 — Hardware Scaling
Compare server-class edge hardware with more constrained devices when available.

## Stage 4 — Alternative Policies
Compare:
1. edge-only
2. cloud-only
3. static split
4. dynamic split
5. phase-aware placement
6. local draft / cloud verify variants if feasible

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
Do not design the final proposed method before baseline measurements establish that the target bottleneck exists.
