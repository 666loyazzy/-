# DynoPipe

## Metadata
- Title: DynoPipe: Heterogeneous Edge-Cloud LLM Serving with Dynamically Orchestrated Pipeline Boundaries
- Venue / Year: ISCA 2026
- Tags: `edge-cloud` `model-partition` `dynamic-scheduling` `pipeline` `wan` `decode`

## 1. Problem
Static edge-cloud partitioning becomes suboptimal when bandwidth, edge compute, memory pressure, and workload change over time.

## 2. Key Idea
DynoPipe pre-computes a small portfolio of split-point configurations and dynamically selects among them at runtime according to live telemetry. A request is constrained to a single Edge→Cloud boundary: stages before the boundary run at the edge and later stages run in the cloud.

## 3. System Design
- Offline profiling of per-layer execution and communication characteristics.
- Dynamic-programming-based construction of candidate split configurations.
- Runtime selection from a small configuration portfolio.
- Hierarchical state management to reduce migration overhead.
- Hysteresis / cooldown to avoid frequent oscillation.

## 4. Experimental Setup
From the paper:
- Edge: RTX 3090 class GPUs
- Cloud: A40 GPU cluster
- Edge-cloud link: 10 Gbps shared uplink
- RTT: roughly 5–50 ms depending on routing/congestion

## 5. Metrics
- Throughput
- TTFT
- TPOT
- E2E latency
- P99 latency
- queueing time

## 6. Main Observation
The paper shows that dynamic split points can outperform static placement under changing load and network conditions. It also reports that pipeline traversal can increase per-token decode latency even when system throughput and queueing behavior improve.

## 7. Strengths
- Targets a real systems problem: volatile heterogeneous resources.
- Treats placement, migration, communication, and runtime adaptation jointly.
- Uses a simple runtime decision path with low online overhead.

## 8. Limitations / Hypotheses to Test
### Explicit structural limitation
The design constrains each request to a single Edge→Cloud boundary.

### Research hypothesis
Because decoder-only LLM generation is autoregressive, placing early layers at the edge and later layers in the cloud may keep WAN communication on the critical path during Decode. This could become unattractive under weaker, higher-RTT, or less stable links than those in the paper's testbed.

This is a **hypothesis to verify experimentally**, not yet a final conclusion.

### Realism question
The reported edge hardware is much stronger than many mobile/embedded edge devices. Re-evaluate conclusions on Jetson/mobile/NPU-class platforms and weaker networks.

## 9. Reproduction Questions
- Can the full system/code be obtained?
- What is the smallest reproducible baseline?
- Can network conditions be emulated with `tc/netem`?
- How do TTFT and TPOT change as RTT grows?
- How many cross-WAN interactions occur per generated token/request?
- How much performance comes from reduced queueing versus faster single-request execution?

## 10. Potential Follow-up Directions
- Phase-aware Prefill/Decode placement.
- Decode-local execution with selective cloud assistance.
- Edge SLM + Cloud LLM collaboration.
- WAN-interaction-aware objective, not only byte-volume-aware placement.
- Dynamic fallback for weak/disconnected networks.
- KV-state placement and migration designed specifically for Decode.

## 11. Advisor Discussion
The advisor specifically highlighted that the work may be relatively shallow and questioned the practicality of Decode remaining dependent on the cloud. Treat this as a direction for literature review and experimental validation rather than as an assumed result.
