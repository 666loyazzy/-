# Taxonomy

This repository classifies Edge-Cloud LLM papers by the **main bottleneck they attack**, not merely by keyword.

## A. Algorithm-Level
### A1. Speculative Decoding
Draft/verify methods that reduce autoregressive decoding cost.

### A2. Self-Speculative Decoding
Uses the target model itself, or a pruned/partial variant, as the draft mechanism.

### A3. Adaptive Inference
Early exit, dynamic depth, token-adaptive execution, or runtime-dependent inference paths.

## B. Model-Level
### B1. Compression
Quantization, pruning, distillation, low-rank approximation.

### B2. KV Cache / Memory
Paged KV, KV compression, placement, eviction, migration, long-context memory control.

### B3. MoE
Expert placement, caching, offloading, substitution, routing, communication reduction.

### B4. Small-Large Model Collaboration
SLM/LLM cooperation beyond classic speculative decoding.

## C. System-Level
### C1. Edge-Cloud Collaborative Inference
Systems where both edge and cloud participate in serving.

### C2. Model Partitioning / Computation Offloading
Layer/operator/graph partitioning and dynamic offload decisions.

### C3. Prefill / Decode Disaggregation
Separates Prefill and Decode placement, scheduling, or resource pools.

### C4. Pipeline / Runtime Scheduling
Runtime orchestration, queueing, batching, placement, migration, and dynamic scheduling.

### C5. Hardware / Compiler / Runtime
GPU/NPU/TPU/Trainium-aware execution, kernels, compilers, runtimes, and heterogeneous execution stacks.

## Cross-Cutting Tags

Use these tags in notes when relevant:

- `edge-cloud`
- `weak-network`
- `prefill`
- `decode`
- `wan`
- `kv-cache`
- `speculative-decoding`
- `moe`
- `dynamic-scheduling`
- `model-partition`
- `offloading`
- `heterogeneous-hardware`
- `energy`
- `privacy`
- `mobile-edge`
- `robotics`

## Inclusion Rule

A paper should be included if it contributes materially to at least one of:

1. efficient on-device LLM inference;
2. edge-cloud collaborative LLM serving;
3. inference techniques directly reusable in edge-cloud systems;
4. hardware/runtime mechanisms that materially change edge deployment feasibility.

Generic datacenter-only papers may still be included when they provide a directly reusable serving mechanism, but should be clearly labeled as background rather than edge-native work.
