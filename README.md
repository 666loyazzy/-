# 论文阅读与研究资料库

仓库导航：[总索引（57 篇）](https://github.com/666loyazzy/research-papers/blob/main/PAPERS.md) · [严格边云（20 篇）](https://github.com/666loyazzy/-/blob/edge-cloud-papers/PAPERS.md) · [辅助知识（25 篇）](https://github.com/666loyazzy/-/blob/other-knowledge/PAPERS.md) · [机器人与 ROS 2（12 篇）](https://github.com/666loyazzy/-/blob/robotics-papers/PAPERS.md)。

本仓库整理严格端/边—云协同 LLM、其它边云与 LLM 系统辅助知识、机器人与 ROS 2 三类资料。`main` 是总入口；本分支保存 DynoPipe 与 16 篇相邻 LLM 系统资料的 17 篇文件副本，以及相关研究笔记。完整论文集合由三个主题分支维护。

## 分支导航

| 分支 | 内容 | 论文数 | 文件 |
|---|---|---:|---|
| [`edge-cloud-papers`](https://github.com/666loyazzy/-/tree/edge-cloud-papers) | 严格端/边—云协同 LLM；含 1 篇保留的历史机制基线 | 20 | 20 篇原文、20 份中文、20 份双语 |
| [`other-knowledge`](https://github.com/666loyazzy/-/tree/other-knowledge) | 16 篇相邻 LLM 系统资料与 9 篇历史 CNN/DNN 资料 | 25 | 25 篇原文、25 份中文、25 份双语 |
| [`robotics-papers`](https://github.com/666loyazzy/-/tree/robotics-papers) | 移动机器人、ROS 2、传感、规划、控制与 SLAM | 12 | 12 篇原文、12 份中文、12 份双语 |

全仓库共 **57 篇不重复论文**：严格边云协同 20 篇、辅助知识 25 篇、机器人与 ROS 2 论文 12 篇。完整清单见 [`PAPERS.md`](PAPERS.md)。原文、中文和双语版，以及跨分支副本，均不重复计数。

## 最新译文

PipeSD 和 SpecEdge 已纳入严格集合，严格集合仍为 20 篇。两篇均提供原版页面内嵌字的中文 PDF 和同页左右对照的双语 PDF，来源与排版检查记录见 [QA 报告](https://github.com/666loyazzy/-/blob/edge-cloud-papers/papers/QA_REPORT.md)。

| 论文 | 中文嵌字版 | 中英双语版 |
|---|---|---|
| PipeSD（ICML 2026） | [中文](https://github.com/666loyazzy/-/blob/edge-cloud-papers/papers/translated/PipeSD_ICML26-mono.pdf) | [双语](https://github.com/666loyazzy/-/blob/edge-cloud-papers/papers/translated/PipeSD_ICML26-dual.pdf) |
| SpecEdge（NeurIPS 2025） | [中文](https://github.com/666loyazzy/-/blob/edge-cloud-papers/papers/translated/SpecEdge_NeurIPS25-mono.pdf) | [双语](https://github.com/666loyazzy/-/blob/edge-cloud-papers/papers/translated/SpecEdge_NeurIPS25-dual.pdf) |

## Strict Edge-Cloud Collaborative LLM Paper Index (20)

以下标题、会议/期刊及顺序与[严格边云主题索引](https://github.com/666loyazzy/-/blob/edge-cloud-papers/PAPERS.md)一致，逐篇原文与译文也从该索引进入。

### A. 顶会/正式发表优先

1. **DynoPipe: Heterogeneous Edge-Cloud LLM Serving with Dynamically Orchestrated Pipeline Boundaries** — ISCA 2026
2. **A Novel Hat-Shaped Device-Cloud Collaborative Inference Framework for Large Language Models (HAT)** — INFOCOM 2026
3. **Crayon: Customized On-Device LLM via Instant Adapter Blending and Edge-Server Hybrid Inference** — ACL 2024
4. **CoGenesis: A Framework Collaborating Large and Small Language Models for Secure Context-Aware Instruction Following** — ACL 2024
5. **Division-of-Thoughts: Harnessing Hybrid Language Model Synergy for Efficient On-Device Agents** — The Web Conference (WWW) 2025
6. **DiSCo: Device-Server Collaborative LLM-Based Text Streaming Services** — Findings of ACL 2025
7. **PipeSD: An Efficient Cloud-Edge Collaborative Pipeline Inference Framework with Speculative Decoding** — ICML 2026
8. **SpecEdge: Scalable Edge-Assisted Serving Framework for Interactive LLMs** — NeurIPS 2025
9. **Ygg: Tree-Based Collaborative Speculative Decoding with Token-Only Transmission** — IEEE/ACM IWQoS 2026
10. **Efficient Deployment of Large Language Model across Cloud-Device Systems** — IEEE SoCC 2024
11. **Splitwise: Collaborative Edge-Cloud Inference for LLMs via Lyapunov-Assisted DRL** — UCC 2025
12. **FlexSpec: Frozen Drafts Meet Evolving Targets in Edge-Cloud Collaborative LLM Speculative Decoding** — IEEE TMC 2026
13. **EdgeShard: Efficient LLM Inference via Collaborative Edge Computing** — IEEE Internet of Things Journal 2025

### B. 严格端/边—云协同 LLM 研究

14. **CE-CoLLM: Efficient and Adaptive Large Language Models Through Cloud-Edge Collaboration** — 2024
15. **CE-LSLM: Efficient Large-Small Language Model Inference and Communication via Cloud-Edge Collaboration** — 2025
16. **PICE: A Semantic-Driven Progressive Inference System for LLM Serving in Cloud-Edge Networks** — 2025
17. **MoA-Off: Adaptive Heterogeneous Modality-Aware Offloading with Edge-Cloud Collaboration for Efficient Multimodal LLM Inference** — 2025
18. **AceSpec: An Asymmetric Edge-Cloud Collaborative Framework for Communication-Efficient LLM Inference** — 2026
19. **Efficient and Privacy-Aware Edge-Cloud Collaborative Inference for Large Language Models (PrivacyAware)** — 2026

### C. 按要求保留的历史机制基线

20. **DynO: Dynamic Onloading of Deep Neural Networks from Cloud to Device** — ACM TECS 2022

## 其它辅助知识（25）

16 篇相邻 LLM 系统资料包括 Splitwise（ISCA 2024，数据中心 Prefill/Decode 拆分）、Helix、TPLA、MuxWise、Past-Future Scheduler、QoServe/Niyama、Shift Parallelism、XY-Serve、Bullet、DynamoLLM、POD-Attention、SwiftSpec、vAttention、AQUA、Kelle 和 llm.npu。

9 篇历史 CNN/DNN 协同资料包括 Neurosurgeon、Edgent、JointDNN、DDNN、BottleNet++、SPINN、CLIO、AppealNet 和 MultiTASC。完整分类与 PDF 见[辅助知识主题索引](https://github.com/666loyazzy/-/blob/other-knowledge/PAPERS.md)。这些工作不计入严格边云协同 20 篇。

## 机器人与 ROS 2（12）

覆盖 PythonRobotics、ROS 2 架构、移动机器人传感、SLAM Toolbox、路径规划、Open3D、Navigation、Pure Pursuit、Kalman Filter、KISS-ICP、ORB-SLAM2 和 SLAM 综述。来源、译文、BibTeX 与阅读提示见[机器人主题索引](https://github.com/666loyazzy/-/blob/robotics-papers/PAPERS.md)。

## 本分支文件

本分支 `papers/` 保存 17 篇资料副本：DynoPipe 1 篇加相邻 LLM 系统资料 16 篇，文件见 [`papers/README.md`](papers/README.md)。其中 DynoPipe 归入严格集合，其余 16 篇归入辅助知识；完整集合分别见对应主题分支。

## 分类与翻译规则

- 严格集合要求端/边与云共同参与同一次 LLM/MLLM 输出；推测解码须有实际的边缘草稿生成与云端目标校验路径。
- 纯数据中心 serving、仅端侧推理、仅云端推理、仅 KV-cache/内存优化及普通 CNN/DNN 背景资料不计入严格集合；DynO 为明确保留的历史机制例外。
- PDF 翻译使用 PDFMathTranslate / pdf2zh，保留公式、图表与原版布局，统一 AI 术语，并检查中文字体嵌入和页面渲染。
- PDF 著作权归原作者及出版机构所有，内容用于个人学习与学术研究。
