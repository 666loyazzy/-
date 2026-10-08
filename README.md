# 论文阅读与研究资料库

本仓库整理三类资料：严格端/边—云协同 LLM、其它边云与 LLM 系统辅助知识、机器人与 ROS 2。`main` 保留跨分支总索引和辅助知识文件；严格边云论文与机器人论文继续放在各自主题分支，原有内容互不混杂。

## 分支导航

| 分支 | 内容 | 论文数 | 说明 |
|---|---|---:|---|
| [`edge-cloud-papers`](https://github.com/666loyazzy/-/tree/edge-cloud-papers) | 严格端/边—云协同 LLM 推理 | 20 | 唯一有效的严格边云集合 |
| [`other-knowledge`](https://github.com/666loyazzy/-/tree/other-knowledge) | LLM serving、端侧推理、数据中心调度与历史机制等辅助知识 | 16 | 原有背景知识保持不变 |
| [`robotics-papers`](https://github.com/666loyazzy/-/tree/robotics-papers) | 移动机器人、ROS 2、传感器、规划、控制、定位与 SLAM | 12 | 原有机器人论文保持不变 |

按主索引统计，共 **48 篇不重复论文**：严格边云协同 20 篇、辅助知识 16 篇、机器人与 ROS 2 论文 12 篇。完整跨分支清单见 [`PAPERS.md`](PAPERS.md)。

## Strict Edge-Cloud Collaborative LLM Paper Index (20)

以下清单是本仓库唯一有效的严格边云协同集合。旧的纯边云清单、PDF 和研究说明不再保留在 `main`，对应资料统一以 `edge-cloud-papers` 分支为准。

### A. 顶会/正式发表优先

1. **DynoPipe: Heterogeneous Edge-Cloud LLM Serving with Dynamically Orchestrated Pipeline Boundaries** — ISCA 2026
2. **A Novel Hat-Shaped Device-Cloud Collaborative Inference Framework for Large Language Models (HAT)** — INFOCOM 2026
3. **Crayon: Customized On-Device LLM via Instant Adapter Blending and Edge-Server Hybrid Inference** — ACL 2024
4. **CoGenesis: A Framework Collaborating Large and Small Language Models for Secure Context-Aware Instruction Following** — ACL 2024
5. **Division-of-Thoughts: Harnessing Hybrid Language Model Synergy for Efficient On-Device Agents** — The Web Conference (WWW) 2025
6. **DiSCo: Device-Server Collaborative LLM-Based Text Streaming Services** — Findings of ACL 2025
7. **Online Scheduling of Battery-Aware Speculative Decoding for Energy-Efficient Cloud-Edge Collaborative LLM Inference** — ICPP 2026
8. **Ygg: Tree-Based Collaborative Speculative Decoding with Token-Only Transmission** — IEEE/ACM IWQoS 2026
9. **Efficient Deployment of Large Language Model across Cloud-Device Systems** — IEEE SoCC 2024
10. **Splitwise: Collaborative Edge-Cloud Inference for LLMs via Lyapunov-Assisted DRL** — UCC 2025
11. **FlexSpec: Frozen Drafts Meet Evolving Targets in Edge-Cloud Collaborative LLM Speculative Decoding** — IEEE TMC 2026
12. **EdgeShard: Efficient LLM Inference via Collaborative Edge Computing** — IEEE Internet of Things Journal 2025

### B. 严格端/边—云协同 LLM 研究

13. **CE-CoLLM: Efficient and Adaptive Large Language Models Through Cloud-Edge Collaboration** — 2024
14. **CE-LSLM: Efficient Large-Small Language Model Inference and Communication via Cloud-Edge Collaboration** — 2025
15. **SplitLLM: Collaborative Inference of LLMs for Model Placement and Request Scheduling** — 2024
16. **PICE: A Semantic-Driven Progressive Inference System for LLM Serving in Cloud-Edge Networks** — 2025
17. **MoA-Off: Adaptive Heterogeneous Modality-Aware Offloading with Edge-Cloud Collaboration for Efficient Multimodal LLM Inference** — 2025
18. **AceSpec: An Asymmetric Edge-Cloud Collaborative Framework for Communication-Efficient LLM Inference** — 2026
19. **Efficient and Privacy-Aware Edge-Cloud Collaborative Inference for Large Language Models (PrivacyAware)** — 2026

### C. 按要求保留的历史机制基线

20. **DynO: Dynamic Onloading of Deep Neural Networks from Cloud to Device** — ACM TECS 2022

严格集合的原文、译文、来源和验收结果见：

- [20 篇完整论文索引](https://github.com/666loyazzy/-/blob/edge-cloud-papers/PAPERS.md)
- [论文官方来源记录](https://github.com/666loyazzy/-/blob/edge-cloud-papers/papers/SOURCES.tsv)
- [PDF 翻译 QA 报告](https://github.com/666loyazzy/-/blob/edge-cloud-papers/papers/QA_REPORT.md)

## 其它辅助知识（16）

`main` 中现有的辅助资料保持不变，包括 Splitwise（数据中心 Prefill/Decode 拆分）、Helix、TPLA、MuxWise、Past-Future Scheduler、QoServe/Niyama、Shift Parallelism、XY-Serve、Bullet、DynamoLLM、POD-Attention、SwiftSpec、vAttention、AQUA、Kelle 和 llm.npu。

这些论文用于理解数据中心 serving、调度、推测解码、KV-cache/内存、端侧推理与硬件机制，不计入严格边云协同 20 篇。文件索引见 [`papers/README.md`](papers/README.md)，主题分支见 [`other-knowledge`](https://github.com/666loyazzy/-/tree/other-knowledge)。

## 机器人与 ROS 2（12）

机器人资料保持原样，覆盖 PythonRobotics、ROS 2 架构、移动机器人传感、SLAM Toolbox、路径规划、Open3D、Navigation、Pure Pursuit、Kalman Filter、KISS-ICP、ORB-SLAM2 和 SLAM 综述。

完整清单见 [`PAPERS.md`](PAPERS.md)，论文文件见 [`robotics-papers`](https://github.com/666loyazzy/-/tree/robotics-papers)。

## 排除规则

以下内容不进入严格边云协同 20 篇集合：

- 纯数据中心 LLM serving；
- 仅端侧推理；
- 仅云端推理；
- 仅 KV-cache 或内存优化。

这些工作若具有背景价值，可保留为辅助知识，但必须与严格边云协同集合分开。

同一篇论文的英文原文、中文单语版和中英双语版只计为 1 篇。PDF 著作权归原作者及出版机构所有，本仓库内容仅用于个人学习与学术研究。
