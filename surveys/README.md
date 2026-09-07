# Survey Workspace — DynoPipe Direction

Working scope: **Dynamic Edge-Cloud LLM Serving and Model Partitioning**.

## Proposed Survey Structure

1. Introduction: why edge-cloud collaborative LLM inference
2. LLM inference background
   - Prefill / Decode
   - KV Cache
   - TTFT / TPOT / throughput / tail latency
3. Static split inference foundations
4. Dynamic model partitioning
   - split-point selection
   - bandwidth / RTT awareness
   - compute / memory awareness
   - mobility-aware partitioning
5. Dynamic pipeline orchestration
   - pipeline construction
   - inflight boundary refactoring
   - compute/communication overlap
6. Runtime placement and offloading
   - heterogeneous resources
   - SLO-aware placement
   - endpoint mobility
7. State and KV-cache migration
8. Realistic WAN evaluation
   - 4G / 5G / Wi-Fi
   - RTT / bandwidth / jitter
   - tail latency
9. DynoPipe as a representative system
   - design
   - optimization assumptions
   - evaluation setup
   - limitations
10. Comparison of DynoPipe-style systems
11. Open problems and experimentable research gaps

## Core Questions

- Is one Edge→Cloud split point sufficient for autoregressive LLM inference?
- Does optimizing communication volume miss communication frequency and RTT sensitivity?
- Should Prefill and Decode use different split/placement strategies?
- How should a system migrate KV/state when the boundary moves?
- How should dynamic partitioning react to network volatility and mobility?
- How realistic are current edge evaluation platforms?
- Which partition/orchestration policies remain useful under weak or intermittent connectivity?

## Writing Rule

The survey should distinguish:
- what a paper explicitly demonstrates;
- what the paper lists as a limitation;
- our own inferred limitation;
- a hypothesis that still requires experiment.

The goal is a **focused map of DynoPipe-style edge-cloud LLM systems**, not a general Edge LLM survey.
