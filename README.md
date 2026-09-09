# 论文阅读与研究资料库

本仓库用于统一整理两个方向的论文资料。`main` 是总入口和完整论文清单；论文 PDF、中文译文、双语版、BibTeX 与阅读笔记分别放在两个主题分支中。

## 分支导航

| 分支 | 内容 | 论文数 | 当前状态 |
|---|---|---:|---|
| [`edge-cloud-papers`](https://github.com/666loyazzy/-/tree/edge-cloud-papers) | 边云协同、异构 LLM 推理、Prefill/Decode、调度与 KV/状态迁移 | 18 | 17 篇已有原文与译文；Tetris 预印本已撤回，保留文献记录 |
| [`robotics-papers`](https://github.com/666loyazzy/-/tree/robotics-papers) | 移动机器人、ROS 2、传感器、规划、控制、定位与 SLAM | 12 | 12 篇原文、12 份中文版、12 份双语版、12 条 BibTeX 与 12 份阅读提示 |

当前总目录共 **30 篇不重复论文**。

## A. 边云协同与异构 LLM 推理（18 篇）

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

[查看边云协同分支的详细索引、原文与译文](https://github.com/666loyazzy/-/blob/edge-cloud-papers/PAPERS.md)

## B. 机器人与 ROS 2 · 第 1 期（12 篇）

| # | 年份 | 主题 | 论文 |
|---:|---:|---|---|
| 1 | 2018 | 机器人算法与 Python 实现 | PythonRobotics: a Python code collection of robotics algorithms |
| 2 | 2022 | ROS 2 的设计与系统架构 | Robot Operating System 2: Design, Architecture, and Uses In The Wild |
| 3 | 2024 | 移动机器人传感器综述 | A Review of Sensing Technologies for Indoor Autonomous Mobile Robots |
| 4 | 2021 | 二维激光建图 | SLAM Toolbox: SLAM for the dynamic world |
| 5 | 2021 | 移动机器人路径规划综述 | Path Planning for Autonomous Mobile Robots: A Review |
| 6 | 2018 | 点云与三维数据处理 | Open3D: A Modern Library for 3D Data Processing |
| 7 | 2020 | Nav2 导航系统与行为树 | The Marathon 2: A Navigation System |
| 8 | 2023 | 路径跟踪与速度调节 | Regulated Pure Pursuit for Robot Path Tracking |
| 9 | 2019 | 卡尔曼滤波的逐步推导 | A Step by Step Mathematical Derivation and Tutorial on Kalman Filters |
| 10 | 2023 | 激光里程计与 ICP 配准 | KISS-ICP: In Defense of Point-to-Point ICP — Simple, Accurate, and Robust Registration If Done the Right Way |
| 11 | 2017 | 视觉 SLAM 系统 | ORB-SLAM2: an Open-Source SLAM System for Monocular, Stereo and RGB-D Cameras |
| 12 | 2016 | SLAM 整体知识框架 | Past, Present, and Future of Simultaneous Localization and Mapping: Towards the Robust-Perception Age |

[查看机器人分支的完整索引、原文、中文译文、双语版与阅读笔记](https://github.com/666loyazzy/-/blob/robotics-papers/PAPERS.md)

## 组织原则

- `main`：只放仓库总介绍、两个方向的完整清单和状态汇总。
- `edge-cloud-papers`：边云协同方向的论文、引用、分类、笔记与研究缺口。
- `robotics-papers`：机器人方向的原文、译文、BibTeX、阅读路线与逐篇笔记。
- 原文优先使用作者主页、会议/期刊页面或 arXiv 等公开来源。
- PDF 翻译使用 PDFMathTranslate / pdf2zh，尽量保留公式、图表与论文布局。
- PDF 著作权归原作者及出版机构所有，仓库内容仅用于个人学习与学术研究。

跨分支文件状态见 [`PAPERS.md`](PAPERS.md)。
