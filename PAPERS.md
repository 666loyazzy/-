# 全仓库论文清单

本文件是 `main` 主干的跨分支总索引。当前共 **30 篇不重复论文**：边云协同 18 篇，机器人与 ROS 2 共 12 篇。

## 分支与资料状态

| 分支 | 篇数 | 原文 / 翻译 / 引用 |
|---|---:|---|
| [`edge-cloud-papers`](https://github.com/666loyazzy/-/tree/edge-cloud-papers) | 18 | 详细下载与翻译状态见该分支 [`PAPERS.md`](https://github.com/666loyazzy/-/blob/edge-cloud-papers/PAPERS.md)；Tetris 预印本已撤回，暂只保留记录 |
| [`robotics-papers`](https://github.com/666loyazzy/-/tree/robotics-papers) | 12 | 12 篇原文、12 份中文版、12 份双语版、完整 BibTeX 与逐篇阅读提示 |

## 边云协同与异构 LLM 推理（18）

1. **DynoPipe: Heterogeneous Edge-Cloud LLM Serving with Dynamically Orchestrated Pipeline Boundaries** — ISCA 2026
2. **Splitwise: Efficient Generative LLM Inference Using Phase Splitting** — ISCA 2024
3. **Helix: Serving Large Language Models over Heterogeneous GPUs and Network via Max-Flow** — ASPLOS 2025
4. **Tetris: Efficient Long-context LLM Serving with Chunkwise Dynamic Sequence Parallelism** — ISCA 2026
5. **TPLA: Tensor Parallel Latent Attention for Efficient Disaggregated Prefill & Decode Inference** — ASPLOS 2026
6. **Towards High-Goodput LLM Serving with Prefill-decode Multiplexing** — ASPLOS 2026
7. **Past-Future Scheduler for LLM Serving under SLA Guarantees** — ASPLOS 2025
8. **QoServe: Breaking the Silos of LLM Inference Serving** — ASPLOS 2026
9. **Shift Parallelism: Low-Latency, High-Throughput LLM Inference for Dynamic Workloads** — ASPLOS 2026
10. **XY-Serve: End-to-End Versatile Production Serving for Dynamic LLM Workloads** — ASPLOS 2026
11. **Boosting GPU Utilization for LLM Serving via Dynamic Spatial-Temporal Orchestration** — ASPLOS 2026
12. **DynamoLLM: Designing LLM Inference Clusters for Performance and Energy Efficiency** — HPCA 2025
13. **POD-Attention: Unlocking Full Prefill-Decode Overlap for Faster LLM Inference** — ASPLOS 2025
14. **SwiftSpec: Disaggregated Speculative Decoding and Fused Kernels for Low-Latency LLM Inference** — ASPLOS 2026
15. **vAttention: Dynamic Memory Management for Serving LLMs without PagedAttention** — ASPLOS 2025
16. **AQUA: Network-Accelerated Memory Offloading for LLMs in Scale-Up GPU Domains** — ASPLOS 2025
17. **Kelle: Co-design KV Caching and eDRAM for Efficient LLM Serving in Edge Computing** — MICRO 2025
18. **Fast On-device LLM Inference with NPUs (llm.npu)** — ASPLOS 2025

## 机器人与 ROS 2 · 论文选读第 1 期（12）

1. **PythonRobotics: a Python code collection of robotics algorithms** — 2018 · 8 页
2. **Robot Operating System 2: Design, Architecture, and Uses In The Wild** — 2022 · 13 页
3. **A Review of Sensing Technologies for Indoor Autonomous Mobile Robots** — 2024 · 31 页
4. **SLAM Toolbox: SLAM for the dynamic world** — 2021 · 7 页
5. **Path Planning for Autonomous Mobile Robots: A Review** — 2021 · 29 页
6. **Open3D: A Modern Library for 3D Data Processing** — 2018 · 6 页
7. **The Marathon 2: A Navigation System** — 2020 · 8 页
8. **Regulated Pure Pursuit for Robot Path Tracking** — 2023 · 11 页
9. **A Step by Step Mathematical Derivation and Tutorial on Kalman Filters** — 2019 · 32 页
10. **KISS-ICP: In Defense of Point-to-Point ICP — Simple, Accurate, and Robust Registration If Done the Right Way** — 2023 · 8 页
11. **ORB-SLAM2: an Open-Source SLAM System for Monocular, Stereo and RGB-D Cameras** — 2017 · 9 页
12. **Past, Present, and Future of Simultaneous Localization and Mapping: Towards the Robust-Perception Age** — 2016 · 作者定稿 24 页

机器人论文的逐篇原文、纯中文嵌字版、中英双语版、来源、引用与推荐读法统一收录在 [`robotics-papers/PAPERS.md`](https://github.com/666loyazzy/-/blob/robotics-papers/PAPERS.md)。

## 计数规则

- 同一篇论文的原文、中文版和双语版只计为 1 篇。
- 主干只汇总，不复制两个分支的大体积 PDF。
- 每一期新增论文时，同时更新本文件、主干 README 和对应主题分支。
