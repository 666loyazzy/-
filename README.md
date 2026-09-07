# Towards Efficient Edge LLM Inference: A Systematic Collection from Algorithm, Model, and System Perspectives

🎉 Welcome! This repository contains papers related to efficient Large Language Model (LLM) inference on edge devices and heterogeneous edge-cloud systems.

🔧 This repository will be **continuously updated and refined** to reflect the latest advancements. If you find any missing papers that are relevant to this repository, we warmly welcome you to **raise a pull request**. We also welcome any suggestions and corrections to help improve the quality and coverage.

💡 If you find this repository helpful, welcome to star and share it with others.

## 👀 Introduction

Large Language Models have rapidly expanded from cloud datacenters toward personal computers, mobile devices, embedded platforms, and heterogeneous edge-cloud systems. However, practical deployment remains challenging because edge devices are constrained by compute capability, memory capacity, energy budget, and network conditions. Recent research therefore explores optimizations across algorithms, models, and systems, including speculative decoding, model compression, Mixture-of-Experts (MoE) execution, model partitioning, computation offloading, dynamic pipeline orchestration, memory management, and hardware-aware acceleration.

In this repository, we categorize existing papers into **algorithm-level, model-level, and system-level optimizations**, with particular attention to edge LLM inference and edge-cloud collaborative serving. The collection is intended to provide a continuously maintained research map for literature review, paper reading, related-work writing, and identifying future research opportunities.

## 📚 Table of Contents

- [👀 Introduction](#-introduction)
- [🧠 Algorithm-Level Optimization](#-algorithm-level-optimization)
  - [Speculative Decoding](#speculative-decoding)
  - [Self-Speculative Decoding](#self-speculative-decoding)
  - [Adaptive Inference](#adaptive-inference)
- [🤖 Model-Level Optimization](#-model-level-optimization)
  - [Model Compression and Quantization](#model-compression-and-quantization)
  - [KV Cache and Memory Optimization](#kv-cache-and-memory-optimization)
  - [Mixture-of-Experts](#mixture-of-experts)
- [⚙️ System-Level Optimization](#-system-level-optimization)
  - [Edge-Cloud Collaborative Inference](#edge-cloud-collaborative-inference)
  - [Model Partitioning and Computation Offloading](#model-partitioning-and-computation-offloading)
  - [Pipeline and Runtime Scheduling](#pipeline-and-runtime-scheduling)
  - [Hardware-Aware Optimization](#hardware-aware-optimization)
- [📌 Citation and Feedback](#-citation-and-feedback)

## 🧠 Algorithm-Level Optimization

### Speculative Decoding

Speculative decoding accelerates autoregressive generation by using a lightweight draft process to propose candidate tokens and a target model to verify them in parallel.

* [arXiv 2022] Fast Inference from Transformers via Speculative Decoding [[paper](https://arxiv.org/abs/2211.17192)]
* [ICML 2023] Accelerating Large Language Model Decoding with Speculative Sampling [[paper](https://arxiv.org/abs/2302.01318)]
* [ICML 2024] EAGLE: Speculative Sampling Requires Rethinking Feature Uncertainty [[paper](https://arxiv.org/abs/2401.15077)] [[code](https://github.com/SafeAILab/EAGLE)]

### Self-Speculative Decoding

Self-speculative decoding reuses a single LLM or a compressed/pruned variant of itself as the draft model, reducing the requirement for an additional separately trained draft model.

* [ISCA 2026] Cassandra: Enabling Reasoning LLMs at Edge via Self-Speculative Decoding [[paper](https://arxiv.org/abs/2605.26558)]

### Adaptive Inference

Adaptive inference dynamically changes model execution according to workload, hardware capability, latency targets, or runtime system conditions.

* More papers will be continuously added.

## 🤖 Model-Level Optimization

### Model Compression and Quantization

Model compression reduces the memory footprint and computational cost of LLM inference through techniques such as pruning, quantization, low-rank approximation, and mixed precision.

* More papers will be continuously added.

### KV Cache and Memory Optimization

KV-cache and memory optimizations reduce the memory bottleneck associated with autoregressive inference, especially for long-context and resource-constrained deployment.

* More papers will be continuously added.

### Mixture-of-Experts

MoE models activate only a subset of experts for each token, providing strong scaling properties but introducing memory, expert placement, communication, and offloading challenges on edge devices.

**Expert offloading and caching:**
* More papers will be continuously added.

**Expert substitution:**
* [ISCA 2026] SMoE: An Algorithm-System Co-Design for Pushing MoE to the Edge via Expert Substitution [[paper](https://arxiv.org/abs/2508.18983)]

## ⚙️ System-Level Optimization

### Edge-Cloud Collaborative Inference

Edge-cloud collaborative inference jointly uses resource-constrained edge devices and more powerful cloud resources to balance latency, throughput, memory usage, energy, and communication cost.

* [ISCA 2026] DynoPipe: Heterogeneous Edge-Cloud LLM Serving with Dynamically Orchestrated Pipeline Boundaries

### Model Partitioning and Computation Offloading

Model partitioning divides LLM computation across devices, while computation offloading determines which parts should execute locally, at the edge, or in the cloud.

* [ISCA 2026] DynoPipe: Heterogeneous Edge-Cloud LLM Serving with Dynamically Orchestrated Pipeline Boundaries

### Pipeline and Runtime Scheduling

Runtime scheduling dynamically coordinates heterogeneous compute, memory, communication, and pipeline resources according to changing system conditions.

* [ISCA 2026] DynoPipe: Heterogeneous Edge-Cloud LLM Serving with Dynamically Orchestrated Pipeline Boundaries

### Hardware-Aware Optimization

Hardware-aware techniques co-design algorithms and systems around GPUs, NPUs, CPUs, memory hierarchies, and device-specific bottlenecks.

* [ISCA 2026] Cassandra: Enabling Reasoning LLMs at Edge via Self-Speculative Decoding [[paper](https://arxiv.org/abs/2605.26558)]
* [ISCA 2026] SMoE: An Algorithm-System Co-Design for Pushing MoE to the Edge via Expert Substitution [[paper](https://arxiv.org/abs/2508.18983)]

## ⭐ Core Papers Currently Being Tracked

* [ISCA 2026] DynoPipe: Heterogeneous Edge-Cloud LLM Serving with Dynamically Orchestrated Pipeline Boundaries
* [ISCA 2026] Cassandra: Enabling Reasoning LLMs at Edge via Self-Speculative Decoding [[paper](https://arxiv.org/abs/2605.26558)]
* [ISCA 2026] SMoE: An Algorithm-System Co-Design for Pushing MoE to the Edge via Expert Substitution [[paper](https://arxiv.org/abs/2508.18983)]

## 📌 Citation and Feedback

This repository is maintained as a continuously updated literature collection for research on efficient Edge LLM inference and heterogeneous edge-cloud LLM systems.

If you find missing papers, incorrect classifications, broken links, or other issues, please feel free to open an issue or submit a pull request.
