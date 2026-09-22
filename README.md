# 论文阅读与研究资料库

本仓库按主题分支整理论文。`main` 是总入口，只汇总目录；PDF 原文、中文嵌字版、双语版和主题资料保存在对应分支。

## 分支导航

| 分支 | 内容 | 论文数 | 状态 |
|---|---|---:|---|
| [`edge-cloud-papers`](https://github.com/666loyazzy/-/tree/edge-cloud-papers) | 严格端/边—云协同 LLM 推理 | 20 | 唯一有效的纯边云协同集合；每篇均有原文、中文单语版和中英双语版 |
| [`other-knowledge`](https://github.com/666loyazzy/-/tree/other-knowledge) | LLM serving、端侧推理、数据中心调度及历史机制等辅助知识 | 16 | 原有背景知识保持不变 |
| [`robotics-papers`](https://github.com/666loyazzy/-/tree/robotics-papers) | 移动机器人、ROS 2、传感器、规划、控制、定位与 SLAM | 12 | 原有机器人论文保持不变 |

按主索引统计，共 **48 篇不重复论文**：严格边云协同 20 篇、其它辅助知识 16 篇、机器人与 ROS 2 论文 12 篇。

## 唯一有效的边云协同集合

纯边云协同分支已经整体替换为 20 篇严格集合：DynoPipe、HAT、Crayon、CoGenesis、Division-of-Thoughts、DiSCo、Battery-Aware Speculative Decoding、Ygg、Efficient Deployment、Splitwise、FlexSpec、EdgeShard、CE-CoLLM、CE-LSLM、SplitLLM、PICE、MoA-Off、AceSpec、PrivacyAware 和作为历史机制基线保留的 DynO。

此前主索引和纯边云分支中的旧清单均已作废；边云协同内容一律以 [`edge-cloud-papers`](https://github.com/666loyazzy/-/tree/edge-cloud-papers) 当前分支为准。

- [20 篇完整论文索引](https://github.com/666loyazzy/-/blob/edge-cloud-papers/PAPERS.md)
- [论文官方来源记录](https://github.com/666loyazzy/-/blob/edge-cloud-papers/papers/SOURCES.tsv)
- [PDF 翻译 QA 报告](https://github.com/666loyazzy/-/blob/edge-cloud-papers/papers/QA_REPORT.md)
- [边云协同分类标准](https://github.com/666loyazzy/-/blob/edge-cloud-papers/TAXONOMY.md)

## 收录原则

- `edge-cloud-papers` 只收录端/边设备与云/服务器共同完成同一次 LLM/MLLM 推理输出的研究。
- 纯数据中心 serving、仅端侧推理、仅云端推理、通用 KV-cache/内存优化及 GPU 集群优化不计入严格边云协同集合。
- 同一篇论文的英文原文、中文单语版和中英双语版只计为 1 篇。
- PDF 著作权归原作者及出版机构所有，本仓库内容仅用于个人学习与学术研究。

跨分支完整清单见 [`PAPERS.md`](PAPERS.md)。
