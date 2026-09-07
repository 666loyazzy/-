# Survey Workspace

Working scope: **Edge-Cloud Collaborative Inference for Large Language Models**.

## Proposed Survey Structure

1. Introduction and motivation
2. LLM inference background
   - Prefill
   - Decode
   - KV Cache
   - TTFT / TPOT / throughput / tail latency
3. Taxonomy
   - algorithm-level
   - model-level
   - system-level
4. Edge-cloud collaborative inference
   - model partitioning
   - computation offloading
   - runtime scheduling
   - dynamic boundaries
5. Decode acceleration and speculative methods
6. KV-cache and memory management
7. MoE on resource-constrained edge systems
8. Prefill/Decode disaggregation and phase-aware systems
9. Evaluation methodology
   - edge hardware realism
   - bandwidth / RTT / jitter
   - workload and concurrency
10. Limitations of current systems
11. Future research directions

## Core Critical Questions

- Is one Edge→Cloud split point sufficient for autoregressive LLM inference?
- Does optimization of communication *volume* miss communication *frequency* and RTT sensitivity?
- Should Prefill and Decode use different placement strategies?
- How realistic are current 'edge' evaluation platforms?
- Which methods remain useful under weak or intermittent connectivity?
- When should systems change the model itself instead of merely changing placement?

## Writing Rule

The survey should distinguish:
- what a paper explicitly demonstrates;
- what the paper itself lists as a limitation;
- our own inferred limitation;
- a hypothesis that still needs experiment.

The goal is not a paper-by-paper summary. The goal is a **research map + comparison + unresolved questions** that can directly guide experiments.
