# DynoPipe-Direction Paper Index — Architecture Top Venues Only

**Venue whitelist:** ISCA / MICRO / HPCA / ASPLOS only.

The list is intentionally narrow. It excludes generic edge AI, pure quantization, unrelated accelerators, generic speculative decoding, and non-top-architecture venues.

## P0 — Directly Closest to DynoPipe

### 1. DynoPipe
**[ISCA 2026] DynoPipe: Heterogeneous Edge-Cloud LLM Serving with Dynamically Orchestrated Pipeline Boundaries**
- DOI: https://doi.org/10.1109/ISCA66397.2026.00077
- Why relevant: exact target paper; dynamic Edge→Cloud boundary selection under heterogeneous and changing resource conditions.
- Key topics: `edge-cloud` `dynamic-partition` `pipeline-boundary` `network-aware` `state-migration`

### 2. Splitwise
**[ISCA 2024] Splitwise: Efficient Generative LLM Inference Using Phase Splitting**
- DOI: https://doi.org/10.1109/ISCA59077.2024.00019
- Paper: https://arxiv.org/abs/2311.18677
- Why relevant: establishes that Prefill and Decode have different resource characteristics and can be placed on separate machines.
- Key topics: `prefill-decode` `phase-splitting` `heterogeneous-hardware` `state-transfer`

### 3. Helix
**[ASPLOS 2025] Helix: Serving Large Language Models over Heterogeneous GPUs and Network via Max-Flow**
- DOI: https://doi.org/10.1145/3669940.3707215
- Paper: https://www.cs.cmu.edu/~rvinayak/papers/Helix_ASPLOS_2025_Serving_LLMs_over_Heterogeneous_GPUs_and_Network_via_Max_Flow.pdf
- Why relevant: jointly optimizes model placement and scheduling while explicitly modeling heterogeneous GPU and network capacities.
- Key topics: `heterogeneous-network` `model-placement` `scheduling` `max-flow`

### 4. Tetris
**[ISCA 2026] Tetris: Efficient Long-context LLM Serving with Chunkwise Dynamic Sequence Parallelism**
- DOI: https://doi.org/10.1109/ISCA66397.2026.00098
- Why relevant: fine-grained runtime adaptation of parallelism under dynamic workloads; useful contrast to DynoPipe's small portfolio of split points.
- Key topics: `dynamic-parallelism` `runtime-adaptation` `prefill-decode` `long-context`

### 5. TPLA
**[ASPLOS 2026] TPLA: Tensor Parallel Latent Attention for Efficient Disaggregated Prefill & Decode Inference**
- Official program: https://www.asplos-conference.org/asplos2026/program/
- Why relevant: directly studies disaggregated Prefill/Decode execution and communication-efficient parallel attention.
- Key topics: `prefill-decode-disaggregation` `tensor-parallel` `communication`

### 6. Prefill-decode Multiplexing
**[ASPLOS 2026] Towards High-Goodput LLM Serving with Prefill-decode Multiplexing**
- Official program: https://www.asplos-conference.org/asplos2026/program/
- Preprint: https://arxiv.org/abs/2504.14489
- Why relevant: dynamically allocates compute between Prefill and Decode instead of treating inference as one homogeneous phase.
- Key topics: `prefill-decode` `dynamic-allocation` `goodput` `resource-multiplexing`

## P1 — Dynamic Scheduling / Runtime Orchestration

### 7. Past-Future Scheduler
**[ASPLOS 2025] Past-Future Scheduler for LLM Serving under SLA Guarantees**
- DOI: https://doi.org/10.1145/3676641.3716011
- Why relevant: scheduling under changing workload and SLA constraints; useful methodology for replacing heuristic thresholding with workload-aware runtime decisions.
- Key topics: `dynamic-scheduling` `SLA` `load-prediction`

### 8. QoServe
**[ASPLOS 2026] QoServe: Breaking the Silos of LLM Inference Serving**
- DOI: https://doi.org/10.1145/3779212.3790206
- Official program: https://www.asplos-conference.org/asplos2026/program/
- Why relevant: dynamically co-schedules requests with different latency requirements while preserving utilization.
- Key topics: `SLO-aware` `dynamic-scheduling` `chunking` `goodput`

### 9. Shift Parallelism
**[ASPLOS 2026] Shift Parallelism: Low-Latency, High-Throughput LLM Inference for Dynamic Workloads**
- Paper: https://arxiv.org/abs/2509.16495
- Official program: https://www.asplos-conference.org/asplos2026/program/
- Why relevant: dynamically switches parallelism modes according to workload conditions; strong comparison point for dynamic runtime reconfiguration.
- Key topics: `dynamic-workload` `parallelism-switching` `runtime-reconfiguration`

### 10. XY-Serve
**[ASPLOS 2026] XY-Serve: End-to-End Versatile Production Serving for Dynamic LLM Workloads**
- Official program: https://www.asplos-conference.org/asplos2026/program/
- Why relevant: production-oriented dynamic LLM serving; useful for understanding robust runtime policies beyond synthetic resource states.
- Key topics: `production-serving` `dynamic-workload` `scheduling`

### 11. Dynamic Spatial-Temporal Orchestration
**[ASPLOS 2026] Boosting GPU Utilization for LLM Serving via Dynamic Spatial-Temporal Orchestration**
- Official program: https://www.asplos-conference.org/asplos2026/program/
- Why relevant: dynamic resource orchestration is conceptually close to DynoPipe's online configuration switching.
- Key topics: `dynamic-orchestration` `GPU-utilization` `resource-allocation`

### 12. DynamoLLM
**[HPCA 2025] DynamoLLM: Designing LLM Inference Clusters for Performance and Energy Efficiency**
- DOI: https://doi.org/10.1109/HPCA61900.2025.00102
- Why relevant: dynamically reconfigures LLM inference clusters under performance constraints; useful as an optimization/control reference.
- Key topics: `dynamic-reconfiguration` `SLO` `energy` `cluster-design`

## P1 — Prefill / Decode and Communication-Critical Execution

### 13. POD-Attention
**[ASPLOS 2025] POD-Attention: Unlocking Full Prefill-Decode Overlap for Faster LLM Inference**
- DOI: https://doi.org/10.1145/3676641.3715996
- Paper: https://arxiv.org/abs/2410.18038
- Why relevant: makes the compute-bound Prefill vs memory-bound Decode distinction concrete and shows how phase overlap changes resource utilization.
- Key topics: `prefill` `decode` `overlap` `attention`

### 14. SwiftSpec
**[ASPLOS 2026] SwiftSpec: Disaggregated Speculative Decoding and Fused Kernels for Low-Latency LLM Inference**
- Official program: https://www.asplos-conference.org/asplos2026/program/
- Why relevant: not a DynoPipe-style layer split, but directly attacks low-latency Decode in a disaggregated setting; useful for the concern that Decode repeatedly crosses a network boundary.
- Key topics: `decode` `disaggregation` `speculative-decoding` `latency`

### 15. TPLA
Already listed in P0 because it is a direct Prefill/Decode disaggregation paper.

## P1 — KV / State / Memory Mechanisms Needed by Dynamic Placement

### 16. vAttention
**[ASPLOS 2025] vAttention: Dynamic Memory Management for Serving LLMs without PagedAttention**
- Paper: https://arxiv.org/abs/2405.04437
- Code: https://github.com/microsoft/vattention
- Why relevant: dynamic placement and migration are constrained by KV-cache memory management; vAttention is a top-venue reference for dynamic KV allocation.
- Key topics: `kv-cache` `dynamic-memory` `runtime`

### 17. Aqua
**[ASPLOS 2025] Aqua: Network-Accelerated Memory Offloading for LLMs in Scale-Up GPU Domains**
- DOI: https://doi.org/10.1145/3676641.3715983
- Why relevant: directly studies network-assisted offloading of LLM memory state; useful when analyzing the true cost of moving state across resource boundaries.
- Key topics: `offloading` `network` `memory` `state-transfer`

### 18. Kelle
**[MICRO 2025] Kelle: Co-design KV Caching and eDRAM for Efficient LLM Serving in Edge Computing**
- DBLP: https://dblp.org/rec/conf/micro/XiaZ25.html
- Why relevant: top-architecture edge-side KV work; useful for testing the alternative design choice of keeping more Decode state local instead of repeatedly depending on cloud execution.
- Key topics: `edge` `kv-cache` `eDRAM` `decode-memory`

## P2 — Edge Reality Check

### 19. llm.npu
**[ASPLOS 2025] Fast On-device LLM Inference with NPUs**
- DOI: https://doi.org/10.1145/3669940.3707239
- Paper: https://arxiv.org/abs/2407.05858
- Why relevant: not cloud-edge collaboration itself, but provides a serious top-venue baseline for what real on-device edge hardware can do, especially Prefill offloading across CPU/GPU/NPU.
- Key topics: `on-device` `NPU` `prefill` `heterogeneous-hardware`

## Reading Order for the Survey

### Round 1 — understand the core problem
1. DynoPipe
2. Splitwise
3. Helix
4. Tetris
5. TPLA
6. Prefill-decode Multiplexing

### Round 2 — understand runtime decision mechanisms
7. Past-Future Scheduler
8. QoServe
9. Shift Parallelism
10. XY-Serve
11. Dynamic Spatial-Temporal Orchestration
12. DynamoLLM

### Round 3 — attack DynoPipe's likely weak point
13. POD-Attention
14. SwiftSpec
15. vAttention
16. Aqua
17. Kelle
18. Fast On-device LLM Inference with NPUs

## Explicitly Excluded

The following are excluded from the core list even if technically interesting:

- OSDI / NSDI / EuroSys / SIGCOMM papers — top systems/networking, but not in the strict architecture whitelist requested here.
- arXiv-only dynamic edge-cloud papers.
- IEEE Access / IoT / general networking journals.
- generic quantization / pruning / MoE papers.
- Cassandra / SMoE unless a later research question specifically requires them.

The repository's main bibliography should remain **small, top-venue, and directly useful for extending or critiquing DynoPipe**.
