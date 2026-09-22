# Taxonomy - Strict Edge-Cloud Collaborative LLM Inference

This repository is intentionally narrow. Except for the explicitly retained DynO historical baseline, a paper is included only when an endpoint/edge model and a cloud/server model jointly contribute to the same LLM/MLLM inference output.

## A. Dynamic Partitioning / Split Computing

Include work that decides where to split the model under changing conditions.

Typical decisions:
- transformer layer / block split point
- edge vs cloud placement
- quantization level coupled with partitioning
- tensor-parallel degree coupled with placement
- split-point adaptation under bandwidth / RTT / compute / memory changes

## B. Computation Offloading / Placement

Include work that dynamically decides which model stages, requests, or dependent models execute on edge vs cloud.

Typical state variables:
- bandwidth
- RTT / jitter
- edge GPU utilization
- memory pressure
- request arrival rate
- mobility
- cloud queue / availability

## C. Dynamic Pipeline Orchestration

Include work on:
- pipeline construction
- moving pipeline boundaries
- inflight pipeline refactoring
- topology-aware pipeline placement
- compute/communication overlap
- reconfiguration stability / hysteresis

## D. State / KV-Cache Migration

Include work on:
- KV-cache migration
- activation/state synchronization
- migration vs recomputation
- geo-distributed endpoint changes
- state continuity during placement changes

## E. Realistic Edge-Cloud Networking

Include work that evaluates or optimizes for:
- WAN RTT
- bandwidth fluctuation
- jitter / packet loss
- 4G / 5G / Wi-Fi
- endpoint mobility
- weak or intermittent connectivity
- P95 / P99 tail latency

## F. Collaborative Generation and Verification

Include work where the two sides jointly produce one result through draft-and-verify, sketch-and-expand, token streaming handoff, subtask decomposition and synthesis, or privacy-preserving knowledge fusion.

Simple whole-request routing is insufficient unless both sides participate in the same request's output path.

## Exclusion Rule

Exclude papers whose main contribution is only:
- speculative decoding wholly inside one cloud/datacenter
- self-speculative decoding
- MoE expert substitution / caching
- quantization / pruning / distillation
- on-device-only LLM inference
- generic compiler / kernel optimization
- generic datacenter serving

unless the paper directly contributes to **cross-boundary generation, verification, partitioning, orchestration, state migration, or WAN-aware serving**.

## Tags

Use only focused tags:

- `dynamic-partition`
- `split-inference`
- `edge-cloud`
- `offloading`
- `pipeline-boundary`
- `dynamic-pipeline`
- `runtime-orchestration`
- `kv-migration`
- `state-migration`
- `wan`
- `weak-network`
- `mobility`
- `prefill`
- `decode`
- `tail-latency`
- `heterogeneous-resources`
- `background`
