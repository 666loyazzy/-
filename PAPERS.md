# Master Paper Index

A compact index. Important papers should also have structured notes under `notes/`.

## Algorithm-Level

### Speculative Decoding
- [arXiv 2022] Fast Inference from Transformers via Speculative Decoding — https://arxiv.org/abs/2211.17192
- [ICML 2023] Accelerating Large Language Model Decoding with Speculative Sampling — https://arxiv.org/abs/2302.01318
- [ICML 2024] EAGLE: Speculative Sampling Requires Rethinking Feature Uncertainty — https://arxiv.org/abs/2401.15077 — code: https://github.com/SafeAILab/EAGLE

### Self-Speculative Decoding
- [ISCA 2026] Cassandra: Enabling Reasoning LLMs at Edge via Self-Speculative Decoding — https://arxiv.org/abs/2605.26558

### Adaptive Inference
- TODO: add representative early-exit / dynamic-depth LLM papers.

## Model-Level

### Compression / Quantization
- TODO: add edge-relevant LLM quantization and pruning papers.

### KV Cache / Memory
- TODO: add PagedAttention/vLLM, KV compression, KV placement, long-context memory papers most relevant to edge deployment.

### Mixture-of-Experts
- [ISCA 2026] SMoE: An Algorithm-System Co-Design for Pushing MoE to the Edge via Expert Substitution — https://arxiv.org/abs/2508.18983
- TODO: add expert offloading, caching, and placement papers.

## System-Level

### Edge-Cloud Collaborative Inference
- [ISCA 2026] DynoPipe: Heterogeneous Edge-Cloud LLM Serving with Dynamically Orchestrated Pipeline Boundaries

### Model Partitioning / Computation Offloading
- [ISCA 2026] DynoPipe: Heterogeneous Edge-Cloud LLM Serving with Dynamically Orchestrated Pipeline Boundaries
- TODO: add static and dynamic LLM partition/offload baselines.

### Prefill / Decode Disaggregation
- TODO: add phase-disaggregated LLM serving papers and edge-cloud variants.

### Pipeline / Runtime Scheduling
- [ISCA 2026] DynoPipe: dynamic boundary orchestration.
- TODO: add representative heterogeneous pipeline and runtime schedulers.

### Hardware / Compiler / Runtime
- [ISCA 2026] Cassandra
- [ISCA 2026] SMoE
- TODO: add mobile GPU/NPU, Jetson, TPU/Trainium, CUDA/MLIR runtime papers that materially affect edge inference.

## Surveys / Collections

- Awesome-PPML-Papers (organization reference): https://github.com/PKU-SEC-Lab/Awesome-PPML-Papers
- TODO: add recent Edge LLM surveys and Edge-Cloud collaborative inference surveys.

## Priority Queue

### P0 — read deeply now
1. DynoPipe
2. Cassandra
3. SMoE

### P1 — needed for the survey next
1. Prefill/Decode disaggregation
2. Distributed / edge-cloud speculative decoding
3. Dynamic model partitioning and offloading
4. KV-cache placement/migration
5. Weak-network / mobile-edge LLM serving

### P2 — background
1. vLLM / PagedAttention
2. continuous batching
3. LLM serving schedulers
4. edge quantization
5. heterogeneous accelerator runtimes
