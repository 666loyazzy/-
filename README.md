# AI Systems & Robotics Paper Library

面向个人科研与课程学习的论文仓库，统一整理两个研究方向：

1. **边云协同与异构 LLM 推理系统**
2. **机器人、定位与 SLAM**

`main` 只作为总入口和完整目录；各方向的论文原文、中文嵌字译文、双语版、引用和阅读笔记分别保存在对应分支中。

## 分支导航

| 分支 | 研究方向 | 清单规模 | PDF / 翻译状态 |
|---|---|---:|---|
| [`edge-cloud-papers`](https://github.com/666loyazzy/-/tree/edge-cloud-papers) | DynoPipe、模型切分、Prefill/Decode、异构调度、KV/状态迁移、端侧推理 | 18 篇 | 17 篇已有原文及中英译文；Tetris 预印本已撤回，暂只保留文献记录 |
| [`robotics-papers`](https://github.com/666loyazzy/-/tree/robotics-papers) | 激光里程计、ICP、视觉 SLAM、SLAM 知识框架 | 3 篇 | 3 篇均有官方原文、纯中文嵌字版、中英双语版、BibTeX 与阅读笔记 |

当前总目录共 **21 篇不重复论文**。

## 完整论文清单

### A. 边云协同与异构 LLM 推理（18 篇）

| # | 年份 / 会议 | 论文 |
|---:|---|---|
| 1 | ISCA 2026 | DynoPipe: Heterogeneous Edge-Cloud LLM Serving with Dynamically Orchestrated Pipeline Boundaries |
| 2 | ISCA 2024 | Splitwise: Efficient Generative LLM Inference Using Phase Splitting |
| 3 | ASPLOS 2025 | Helix: Serving Large Language Models over Heterogeneous GPUs and Network via Max-Flow |
| 4 | ISCA 2026 | Tetris: Efficient Long-context LLM Serving with Chunkwise Dynamic Sequence Parallelism |
| 5 | ASPLOS 2026 | TPLA: Tensor Parallel Latent Attention for Efficient Disaggregated Prefill & Decode Inference |
| 6 | ASPLOS 2026 | Towards High-Goodput LLM Serving with Prefill-decode Multiplexing |
| 7 | ASPLOS 2025 | Past-Future Scheduler for LLM Serving under SLA Guarantees |
| 8 | ASPLOS 2026 | QoServe: Breaking the Silos of LLM Inference Serving |
| 9 | ASPLOS 2026 | Shift Parallelism: Low-Latency, High-Throughput LLM Inference for Dynamic Workloads |
| 10 | ASPLOS 2026 | XY-Serve: End-to-End Versatile Production Serving for Dynamic LLM Workloads |
| 11 | ASPLOS 2026 | Boosting GPU Utilization for LLM Serving via Dynamic Spatial-Temporal Orchestration |
| 12 | HPCA 2025 | DynamoLLM: Designing LLM Inference Clusters for Performance and Energy Efficiency |
| 13 | ASPLOS 2025 | POD-Attention: Unlocking Full Prefill-Decode Overlap for Faster LLM Inference |
| 14 | ASPLOS 2026 | SwiftSpec: Disaggregated Speculative Decoding and Fused Kernels for Low-Latency LLM Inference |
| 15 | ASPLOS 2025 | vAttention: Dynamic Memory Management for Serving LLMs without PagedAttention |
| 16 | ASPLOS 2025 | AQUA: Network-Accelerated Memory Offloading for LLMs in Scale-Up GPU Domains |
| 17 | MICRO 2025 | Kelle: Co-design KV Caching and eDRAM for Efficient LLM Serving in Edge Computing |
| 18 | ASPLOS 2025 | Fast On-device LLM Inference with NPUs (llm.npu) |

[查看边云协同详细索引、原文与译文](https://github.com/666loyazzy/-/blob/edge-cloud-papers/PAPERS.md)

### B. 机器人与 SLAM（3 篇）

| # | 主题 | 年份 | 论文 |
|---:|---|---:|---|
| 1 | 激光里程计与 ICP 配准 | 2023 | KISS-ICP: In Defense of Point-to-Point ICP — Simple, Accurate, and Robust Registration If Done the Right Way |
| 2 | 视觉 SLAM 系统 | 2017 | ORB-SLAM2: an Open-Source SLAM System for Monocular, Stereo and RGB-D Cameras |
| 3 | SLAM 整体知识框架 | 2016 | Past, Present, and Future of Simultaneous Localization and Mapping: Towards the Robust-Perception Age |

[查看机器人论文详细索引、官方原文、中文译文与阅读笔记](https://github.com/666loyazzy/-/blob/robotics-papers/PAPERS.md)

## 仓库组织原则

- `main`：总介绍、跨分支完整论文清单与状态汇总。
- `edge-cloud-papers`：边云协同方向的原文、译文、引用、分类、阅读笔记和研究缺口。
- `robotics-papers`：机器人方向的原文、译文、引用与入门阅读路线。
- 原文优先使用作者主页、会议页面或 arXiv 等公开来源。
- PDF 翻译使用 PDFMathTranslate / pdf2zh，尽量保留公式、图表和论文布局。
- PDF 著作权归原作者及出版机构所有，仓库内容仅用于个人学习与学术研究。

更详细的跨分支状态请见 [PAPERS.md](PAPERS.md)。
