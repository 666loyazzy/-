# Awesome Edge-Cloud LLM Papers

A continuously maintained research map for **efficient LLM inference on edge devices and heterogeneous edge-cloud systems**.

This repository is organized for three purposes:
1. build a literature review quickly;
2. keep structured reading notes instead of loose bookmarks;
3. track research gaps that can later become experiments and papers.

> Current focus: **Edge-Cloud LLM Serving**, especially dynamic partitioning, Prefill/Decode placement, speculative decoding, KV-cache management, MoE execution, runtime scheduling, and realistic weak-network edge scenarios.

## Research Map

### 1. Algorithm-Level Optimization
- Speculative Decoding
- Self-Speculative Decoding
- Adaptive / Early-Exit Inference

### 2. Model-Level Optimization
- Quantization / Pruning / Distillation
- KV Cache and Memory Optimization
- Mixture-of-Experts
- Small-Large Model Collaboration

### 3. System-Level Optimization
- Edge-Cloud Collaborative Inference
- Model Partitioning and Computation Offloading
- Prefill / Decode Disaggregation
- Pipeline and Runtime Scheduling
- Heterogeneous Hardware / Compiler / Runtime

## Core Papers Being Tracked

### Edge-Cloud Collaborative Inference
- **[ISCA 2026] DynoPipe: Heterogeneous Edge-Cloud LLM Serving with Dynamically Orchestrated Pipeline Boundaries** — dynamic Edge→Cloud split point; current main baseline and discussion target. See [note](notes/DynoPipe.md).

### Self-Speculative Decoding
- **[ISCA 2026] Cassandra: Enabling Reasoning LLMs at Edge via Self-Speculative Decoding** — [[paper](https://arxiv.org/abs/2605.26558)] — see [note](notes/Cassandra.md).

### MoE on Edge
- **[ISCA 2026] SMoE: An Algorithm-System Co-Design for Pushing MoE to the Edge via Expert Substitution** — [[paper](https://arxiv.org/abs/2508.18983)] — see [note](notes/SMoE.md).

### Speculative Decoding Foundations
- **[arXiv 2022] Fast Inference from Transformers via Speculative Decoding** — [[paper](https://arxiv.org/abs/2211.17192)]
- **[ICML 2023] Accelerating Large Language Model Decoding with Speculative Sampling** — [[paper](https://arxiv.org/abs/2302.01318)]
- **[ICML 2024] EAGLE: Speculative Sampling Requires Rethinking Feature Uncertainty** — [[paper](https://arxiv.org/abs/2401.15077)] [[code](https://github.com/SafeAILab/EAGLE)]

## Current Research Question

A central question motivating this collection is:

> **How should Prefill and Decode be placed and orchestrated across edge and cloud under realistic bandwidth, RTT, memory, and compute constraints?**

A particularly important limitation to investigate is whether layer-wise Edge→Cloud partitioning makes autoregressive Decode too dependent on WAN communication. This is tracked as a hypothesis, not a conclusion, in [research-gaps/README.md](research-gaps/README.md).

## Repository Structure

```text
.
├── README.md
├── PAPERS.md                  # master literature index
├── TAXONOMY.md                # classification rules
├── notes/
│   ├── TEMPLATE.md
│   ├── DynoPipe.md
│   ├── Cassandra.md
│   └── SMoE.md
├── surveys/
│   └── README.md
├── experiments/
│   └── README.md
└── research-gaps/
    └── README.md
```

## Reading-Note Standard

For every important paper, record:

**Problem | Key Idea | System Design | Model | Edge Hardware | Cloud Hardware | Network | Metrics | Baselines | Main Results | Limitations | Relation to DynoPipe | Reproduction Status | Research Opportunities**

Use [notes/TEMPLATE.md](notes/TEMPLATE.md) for new papers.

## Metrics We Care About

- TTFT — Time To First Token
- TPOT — Time Per Output Token
- End-to-End Latency
- P50 / P95 / P99 Latency
- Throughput / Tokens per Second
- Edge Memory Footprint
- Communication Volume
- Number of WAN Interactions per Generated Token / Request
- Energy / Power
- Accuracy / Acceptance Rate where applicable

## Maintenance Rule

When adding a paper:
1. place it in the correct taxonomy section in `PAPERS.md`;
2. add `paper` / `code` links when available;
3. create a structured note for important papers;
4. label unverified ideas as **hypotheses** rather than facts;
5. prioritize peer-reviewed papers and official artifacts over secondary summaries.

## Status

This repository is currently in the **literature-review stage**. The next milestone is to expand the paper map, compare representative systems under a unified taxonomy, and then convert high-confidence gaps into reproducible experiments.
