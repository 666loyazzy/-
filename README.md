# Awesome DynoPipe-Style Edge-Cloud LLM Papers

A focused literature repository for the **DynoPipe research direction**: dynamic edge-cloud LLM serving, model partitioning, computation offloading, pipeline-boundary adaptation, runtime orchestration, and state migration under heterogeneous and time-varying network/compute resources.

> **Scope rule:** this repo does **not** collect generic Edge LLM papers. Pure on-device quantization, MoE, speculative decoding, and unrelated hardware/compiler papers are excluded unless they directly solve an edge-cloud partitioning / orchestration problem.

## Core Research Question

> How should an LLM be dynamically partitioned and orchestrated across edge and cloud when bandwidth, RTT, edge compute, memory, workload, and endpoint location change over time?

The main baseline is **DynoPipe (ISCA 2026)**. A particularly important open question is whether a single Edge→Cloud pipeline boundary makes autoregressive Decode overly dependent on WAN communication.

## Research Map

### A. Dynamic Edge-Cloud Model Partitioning
- dynamic split-point selection
- layer / block placement
- computation offloading
- network-aware and mobility-aware partitioning
- joint partition + quantization / resource allocation

### B. Edge-Cloud LLM Serving & Resource Orchestration
- heterogeneous edge-cloud serving
- workload-aware orchestration
- SLO-aware placement
- endpoint mobility
- multi-model / multi-node deployment

### C. Dynamic Pipeline Refactoring
- pipeline construction
- pipeline-boundary movement
- inflight reconfiguration
- computation/communication overlap

### D. State & KV-Cache Migration
- KV-cache placement and migration
- state synchronization
- migration-vs-recomputation trade-offs
- geo-distributed serving

### E. Weak-Network / Realistic Edge Evaluation
- WAN RTT / bandwidth / jitter
- 4G / 5G / Wi-Fi traces
- tail latency
- edge mobility
- degraded / intermittent connectivity

## P0 — Must Read

1. **[ISCA 2026] DynoPipe: Heterogeneous Edge-Cloud LLM Serving with Dynamically Orchestrated Pipeline Boundaries** — main baseline.
2. **[EuroSys 2026] FlexPipe: Adapting Dynamic LLM Serving Through Inflight Pipeline Refactoring in Fragmented Serverless Clusters** — same research lineage; dynamic pipeline refactoring.
3. **[SIGCOMM 2026] Connex: Endpoint Mobility Primitives for Dynamic LLM Serving** — same research lineage; mobility/network dimension of dynamic serving.
4. **[WcCST 2026] DynaSplit: Latency-Aware Dynamic Model Partitioning for Large Language Model Inference in the Edge-Cloud Continuum** — direct dynamic partitioning competitor.
5. **[FITEE 2025] Adaptive Layer Splitting for Wireless Large Language Model Inference in Edge Computing: A Model-Based Reinforcement Learning Approach** — wireless/network-aware LLM split inference.
6. **[ICDCS 2026] Efficient KV Cache Migration for Geo-Distributed LLM Inference in Collaborative Edge Computing** — state migration, directly relevant to boundary movement.

## P1 — Directly Relevant

- **[ICC 2025] Distributed Inference Optimization for Large Language Model in Edge-Cloud Collaborative Networks**
- **[arXiv 2025] Memory- and Latency-Constrained Inference of Large Language Models via Adaptive Split Computing**
- **[arXiv 2025] Splitwise: Collaborative Edge-Cloud Inference for LLMs via Lyapunov-Assisted DRL**
- **[Electronics 2025] DAPO: Mobility-Aware Joint Optimization of Model Partitioning and Task Offloading for Edge LLM Inference**
- **[ACL 2026] EdgeFormer: Latency-Aware Collaborative Multi-Head Attention of Transformer Inference in Edge Networks**
- **[ICDCS 2026] TurboInfer: Targeting Age of Model Inference Optimization for Joint Model Inference in Edge Cloud Systems**
- **[arXiv 2026] Efficient and Privacy Aware Edge Cloud Collaborative Inference for Large Language Models**

See [`PAPERS.md`](PAPERS.md) for links and classification.

## Explicitly Out of Scope

The following are **not core papers for this repo** unless they directly connect to edge-cloud partition/orchestration:

- Cassandra / generic self-speculative decoding
- SMoE / generic expert substitution
- generic LLM quantization/pruning
- generic on-device-only LLM inference
- datacenter-only serving papers with no transferable partition/orchestration mechanism

## Repository Structure

```text
.
├── README.md
├── PAPERS.md
├── TAXONOMY.md
├── notes/
│   ├── TEMPLATE.md
│   └── DynoPipe.md
├── surveys/
│   └── README.md
├── experiments/
│   └── README.md
└── research-gaps/
    └── README.md
```

## Reading-Note Standard

For every important paper, record:

**Problem | Split / Placement Decision | Online State | Optimization Method | Edge Hardware | Cloud Hardware | Network | Prefill/Decode Behavior | KV/State Handling | Metrics | Baselines | Main Results | Limitations | Relation to DynoPipe | Reproduction Status | Research Gap**

## Metrics We Care About

- TTFT
- TPOT
- end-to-end latency
- P95 / P99 tail latency
- throughput
- edge memory footprint
- activation / KV communication volume
- WAN interactions per request / generated token
- migration overhead
- bandwidth / RTT sensitivity
- robustness under jitter / mobility / weak network

## Current Hypothesis to Verify

DynoPipe constrains each request to a single Edge→Cloud split point. For autoregressive generation, this may place WAN communication repeatedly on the Decode critical path. The repository will treat this as a **testable hypothesis**, not a conclusion, and prioritize papers and experiments that can confirm, refine, or refute it.
