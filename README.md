# 论文阅读与研究资料库

本仓库按主题分支整理论文。`main` 是总入口；PDF 原文、中文嵌字版、双语版和主题资料保存在对应分支。

## 分支导航

| 分支 | 范围 | 论文数 | 状态 |
|---|---|---:|---|
| [`edge-cloud-papers`](https://github.com/666loyazzy/-/tree/edge-cloud-papers) | 严格边云协同：端/边与云之间存在真实的切分、路由、卸载、流水线或状态交换 | 20 | 20 篇原文、20 份中文单语版、20 份中英双语版；含术语表、来源表和 QA 报告 |
| [`other-knowledge`](https://github.com/666loyazzy/-/tree/other-knowledge) | 与 LLM serving、端侧推理、数据中心调度等有关，但不满足严格边云协同定义 | 16 | 保留原有原文和译文，作为背景知识 |
| [`robotics-papers`](https://github.com/666loyazzy/-/tree/robotics-papers) | 移动机器人、ROS 2、传感器、规划、控制、定位与 SLAM | 12 | 12 篇原文、中文版、双语版、BibTeX 与阅读提示 |

当前总目录共 **48 篇不重复论文**。

## 严格边云协同集合

严格集合包含 DynoPipe、Neurosurgeon、Edgent、JointDNN、DDNN、BottleNet++、SPINN、CLIO、AppealNet、DynO、MultiTASC、EdgeShard、CE-CoLLM、HAT、CE-LSLM、SplitLLM、MoA-Off、AceSpec、Privacy-Aware Edge-Cloud LLM 和一篇 Edge SLM–Cloud LLM 综述。

- [完整论文索引](https://github.com/666loyazzy/-/blob/edge-cloud-papers/PAPERS.md)
- [官方来源记录](https://github.com/666loyazzy/-/blob/edge-cloud-papers/papers/SOURCES.tsv)
- [PDF 翻译 QA 报告](https://github.com/666loyazzy/-/blob/edge-cloud-papers/papers/QA_REPORT.md)

## 分类原则

- `edge-cloud-papers` 只收录真实跨端/边—云协同执行的论文。
- 纯数据中心 serving、仅端侧推理、仅 KV-cache/内存优化、仅 speculative decoding、仅 GPU 内并行等论文放入 `other-knowledge`。
- 同一篇论文的英文原文、中文单语版和中英双语版只计为 1 篇。
- 原文优先使用作者主页、会议/期刊页面或 arXiv 等公开来源。
- PDF 翻译使用 PDFMathTranslate / pdf2zh，保留公式、图表和论文布局；AI 术语按领域语义统一，并检查中文字体嵌入与逐页渲染。
- PDF 著作权归原作者及出版机构所有，仓库内容仅用于个人学习与学术研究。

跨分支完整清单见 [`PAPERS.md`](PAPERS.md)。
