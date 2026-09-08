# Awesome DynoPipe-Direction Papers

A strictly curated literature repository for the **DynoPipe research direction**: dynamic LLM serving across heterogeneous compute and network resources, with emphasis on **model partitioning, computation offloading, prefill/decode placement, pipeline orchestration, runtime scheduling, KV/state movement, and WAN/network sensitivity**.

## Repository Branches

- [`edge-cloud-papers`](https://github.com/666loyazzy/-/tree/edge-cloud-papers) - DynoPipe / 边云协同论文库
- [`robotics-papers`](https://github.com/666loyazzy/-/tree/robotics-papers) - 机器人与 SLAM 论文库（官方原文、中文译文、双语版与 BibTeX）

## Venue Policy

This repository now uses a **strict computer-architecture top-venue whitelist**:

- **ISCA** — International Symposium on Computer Architecture
- **MICRO** — IEEE/ACM International Symposium on Microarchitecture
- **HPCA** — IEEE International Symposium on High Performance Computer Architecture
- **ASPLOS** — Architectural Support for Programming Languages and Operating Systems

Papers from OSDI, NSDI, EuroSys, SIGCOMM, MLSys, arXiv-only venues, IEEE Access, IoT journals, etc. are **not included in the main list**, even when technically relevant. They may be kept separately later as background, but not mixed into the core bibliography.

## Scope

A paper is included only if it materially helps answer at least one of these questions:

1. Where should LLM computation run under heterogeneous compute/network conditions?
2. How should a model or inference phase be partitioned across resources?
3. How should runtime orchestration adapt to changing load, bandwidth, latency, or memory pressure?
4. How should Prefill and Decode be separated, overlapped, or migrated?
5. How can KV-cache / inference state be moved or managed cheaply enough to support dynamic placement?
6. How realistic is edge-side execution when compared with datacenter-class assumptions?

## Must-Read Core

1. **[ISCA 2026] DynoPipe: Heterogeneous Edge-Cloud LLM Serving with Dynamically Orchestrated Pipeline Boundaries**  
   Core target paper. Dynamic Edge→Cloud split point under changing bandwidth/compute/memory conditions.

2. **[ISCA 2024] Splitwise: Efficient Generative LLM Inference Using Phase Splitting**  
   Separates prompt computation and token generation onto different machines; foundational for thinking about Prefill/Decode-aware placement.

3. **[ASPLOS 2025] Helix: Serving Large Language Models over Heterogeneous GPUs and Network via Max-Flow**  
   Jointly models heterogeneous GPUs and network links; optimizes model placement and scheduling using a graph/max-flow formulation.

4. **[ISCA 2026] Tetris: Efficient Long-context LLM Serving with Chunkwise Dynamic Sequence Parallelism**  
   Dynamically changes parallelism at fine granularity under varying workloads; useful for understanding runtime adaptation beyond a fixed split point.

5. **[ASPLOS 2026] TPLA: Tensor Parallel Latent Attention for Efficient Disaggregated Prefill & Decode Inference**  
   Directly relevant to disaggregated Prefill/Decode execution and cross-resource communication.

6. **[ASPLOS 2026] Towards High-Goodput LLM Serving with Prefill-decode Multiplexing**  
   Dynamically multiplexes Prefill and Decode resources and directly addresses the phase-allocation problem.

7. **[ASPLOS 2025] POD-Attention: Unlocking Full Prefill-Decode Overlap for Faster LLM Inference**  
   Shows why Prefill and Decode have different bottlenecks and how their overlap can be exploited at the kernel/resource level.

8. **[ASPLOS 2025] Past-Future Scheduler for LLM Serving under SLA Guarantees**  
   Dynamic scheduling under changing request conditions and latency constraints.

9. **[ASPLOS 2026] QoServe: Breaking the Silos of LLM Inference Serving**  
   SLO-aware dynamic scheduling across heterogeneous request classes.

10. **[MICRO 2025] Kelle: Co-design KV Caching and eDRAM for Efficient LLM Serving in Edge Computing**  
    Important edge-side memory/KV reference for judging whether Decode can realistically stay local.

## Why This Set Matters for DynoPipe

The core research line is not generic "edge LLM". It is:

```text
heterogeneous resources
        ↓
model / phase placement
        ↓
network + compute + memory bottlenecks
        ↓
dynamic runtime adaptation
        ↓
state / KV movement
        ↓
TTFT / TPOT / throughput / tail latency
```

The current working hypothesis is that **single-boundary Edge→Cloud partitioning may remain too WAN-dependent during autoregressive Decode**, so papers on Prefill/Decode disaggregation, heterogeneous placement, dynamic scheduling, and KV-state management are especially important.

## Repository Files

- [`PAPERS.md`](PAPERS.md) — strict top-venue paper index with relevance labels
- [`papers/README.md`](papers/README.md) — source PDFs, provenance, and translation status
- [`TAXONOMY.md`](TAXONOMY.md) — DynoPipe-specific classification rules
- [`notes/DynoPipe.md`](notes/DynoPipe.md) — current core reading note
- [`research-gaps/README.md`](research-gaps/README.md) — testable hypotheses
- [`experiments/README.md`](experiments/README.md) — future reproduction/evaluation plan

## Current Reading Order

**DynoPipe → Splitwise → Helix → Tetris → TPLA → Prefill-decode Multiplexing → POD-Attention → Past-Future Scheduler → QoServe → Kelle**

This order moves from the exact target paper to the closest architectural mechanisms needed to critique and extend it.
