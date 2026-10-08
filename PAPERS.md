# 全仓库论文清单

当前按主索引统计共 **48 篇不重复论文**：严格边云协同 20 篇、其它辅助知识 16 篇、机器人与 ROS 2 论文 12 篇。

## A. 严格边云协同 LLM（20）

1. **DynoPipe: Heterogeneous Edge-Cloud LLM Serving with Dynamically Orchestrated Pipeline Boundaries** — ISCA 2026
2. **A Novel Hat-Shaped Device-Cloud Collaborative Inference Framework for Large Language Models (HAT)** — INFOCOM 2026
3. **Crayon: Customized On-Device LLM via Instant Adapter Blending and Edge-Server Hybrid Inference** — ACL 2024
4. **CoGenesis: A Framework Collaborating Large and Small Language Models for Secure Context-Aware Instruction Following** — ACL 2024
5. **Division-of-Thoughts: Harnessing Hybrid Language Model Synergy for Efficient On-Device Agents** — WWW 2025
6. **DiSCo: Device-Server Collaborative LLM-Based Text Streaming Services** — Findings of ACL 2025
7. **Online Scheduling of Battery-Aware Speculative Decoding for Energy-Efficient Cloud-Edge Collaborative LLM Inference** — ICPP 2026
8. **Ygg: Tree-Based Collaborative Speculative Decoding with Token-Only Transmission** — IEEE/ACM IWQoS 2026
9. **Efficient Deployment of Large Language Model across Cloud-Device Systems** — IEEE SoCC 2024
10. **Splitwise: Collaborative Edge-Cloud Inference for LLMs via Lyapunov-Assisted DRL** — UCC 2025
11. **FlexSpec: Frozen Drafts Meet Evolving Targets in Edge-Cloud Collaborative LLM Speculative Decoding** — IEEE TMC 2026
12. **EdgeShard: Efficient LLM Inference via Collaborative Edge Computing** — IEEE Internet of Things Journal 2025
13. **CE-CoLLM: Efficient and Adaptive Large Language Models Through Cloud-Edge Collaboration** — 2024
14. **CE-LSLM: Efficient Large-Small Language Model Inference and Communication via Cloud-Edge Collaboration** — 2025
15. **SplitLLM: Collaborative Inference of LLMs for Model Placement and Request Scheduling** — 2024
16. **PICE: A Semantic-Driven Progressive Inference System for LLM Serving in Cloud-Edge Networks** — 2025
17. **MoA-Off: Adaptive Heterogeneous Modality-Aware Offloading with Edge-Cloud Collaboration for Efficient Multimodal LLM Inference** — 2025
18. **AceSpec: An Asymmetric Edge-Cloud Collaborative Framework for Communication-Efficient LLM Inference** — 2026
19. **Efficient and Privacy-Aware Edge-Cloud Collaborative Inference for Large Language Models (PrivacyAware)** — 2026
20. **DynO: Dynamic Onloading of Deep Neural Networks from Cloud to Device** — ACM TECS 2022（按要求保留的历史机制基线）

[查看原文、译文、来源与验收结果](https://github.com/666loyazzy/-/blob/edge-cloud-papers/PAPERS.md)

## B. 其它辅助知识（16）

1. **Splitwise** — 数据中心 Prefill/Decode 阶段拆分
2. **Helix** — 异构数据中心 GPU 放置与网络调度
3. **TPLA** — 数据中心解耦式 Prefill/Decode 张量并行
4. **MuxWise** — 数据中心 Prefill/Decode 资源复用
5. **Past-Future Scheduler** — 数据中心 SLA 感知请求调度
6. **QoServe / Niyama** — 数据中心推理协同调度与隔离
7. **Shift Parallelism** — 数据中心动态工作负载并行策略切换
8. **XY-Serve** — 生产环境数据中心 LLM serving
9. **Bullet** — 数据中心 GPU 时空编排
10. **DynamoLLM** — 数据中心推理集群设计与重配置
11. **POD-Attention** — GPU 内核级 Prefill/Decode 重叠
12. **SwiftSpec** — 服务器基础设施内的解耦式推测解码
13. **vAttention** — 数据中心 KV cache 虚拟内存管理
14. **AQUA** — Scale-up GPU 域内存卸载
15. **Kelle** — 无云侧协同执行的边缘 KV/eDRAM 设计
16. **llm.npu** — 纯端侧异构 NPU 推理

[查看辅助知识分支](https://github.com/666loyazzy/-/blob/other-knowledge/PAPERS.md)

## C. 机器人与 ROS 2（12）

1. **PythonRobotics: a Python code collection of robotics algorithms** — 2018
2. **Robot Operating System 2: Design, Architecture, and Uses In The Wild** — 2022
3. **A Review of Sensing Technologies for Indoor Autonomous Mobile Robots** — 2024
4. **SLAM Toolbox: SLAM for the dynamic world** — 2021
5. **Path Planning for Autonomous Mobile Robots: A Review** — 2021
6. **Open3D: A Modern Library for 3D Data Processing** — 2018
7. **The Marathon 2: A Navigation System** — 2020
8. **Regulated Pure Pursuit for Robot Path Tracking** — 2023
9. **A Step by Step Mathematical Derivation and Tutorial on Kalman Filters** — 2019
10. **KISS-ICP: In Defense of Point-to-Point ICP — Simple, Accurate, and Robust Registration If Done the Right Way** — 2023
11. **ORB-SLAM2: an Open-Source SLAM System for Monocular, Stereo and RGB-D Cameras** — 2017
12. **Past, Present, and Future of Simultaneous Localization and Mapping: Towards the Robust-Perception Age** — 2016

[查看机器人分支](https://github.com/666loyazzy/-/blob/robotics-papers/PAPERS.md)

## 计数与维护规则

- 同一篇论文的原文、中文版和双语版只计为 1 篇。
- `main` 只维护跨分支总索引，不复制主题分支的大体积 PDF。
- 纯边云协同内容以 `edge-cloud-papers` 当前 20 篇清单为唯一标准。
- `other-knowledge` 和 `robotics-papers` 的现有资料保持独立，不因纯边云集合替换而改动。
