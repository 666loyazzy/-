# Strict Edge-Cloud Collaborative LLM Papers

仓库导航：[总索引（57 篇）](https://github.com/666loyazzy/research-papers/blob/main/PAPERS.md) · [严格边云（20 篇）](https://github.com/666loyazzy/-/blob/edge-cloud-papers/PAPERS.md) · [辅助知识（25 篇）](https://github.com/666loyazzy/-/blob/other-knowledge/PAPERS.md) · [机器人与 ROS 2（12 篇）](https://github.com/666loyazzy/-/blob/robotics-papers/PAPERS.md)。

本分支只收录端/边设备与云/服务器共同完成同一次 LLM/MLLM 推理输出的论文。标题里出现 `edge`、单纯把请求路由到某一侧、纯端侧推理、纯云端 serving、通用 KV-cache/内存/GPU 集群优化都不计入。

## 当前规模

- 严格清单：20 篇研究论文，恰好 20 篇
- 明确保留：DynoPipe、DynO、PrivacyAware
- LLM/MLLM 严格协同：19 篇；DynO 按要求作为历史机制基线保留 1 篇
- 正式会议/期刊论文优先：ISCA、ICML、NeurIPS、INFOCOM、ACL、WWW、IWQoS、SoCC、UCC、IEEE TMC、IEEE IoT Journal 等
- 每篇均提供公开原文、中文嵌字版（`-mono.pdf`）和中英双语版（`-dual.pdf`）
- 最新收录：PipeSD（ICML 2026）与 SpecEdge（NeurIPS 2025），严格清单仍为 20 篇

## 核心研究线

1. 边缘草稿模型与云端目标模型的协同推测解码，包括 PipeSD 的 token 批次流水线调度与 SpecEdge 的主动式边缘草稿生成、服务器流水线感知调度
2. 设备/服务器跨边界流水线、动态切分与算子级调度
3. 端侧 SLM 与云侧 LLM 的分解、生成、校验与融合
4. 带宽、RTT、能耗、负载和模型演化感知的运行时调度
5. 隐私感知的端云协同生成

完整清单、来源和分类见 [`PAPERS.md`](PAPERS.md)、[`papers/SOURCES.tsv`](papers/SOURCES.tsv) 与 [`TAXONOMY.md`](TAXONOMY.md)。

PDF 著作权归原作者及出版机构所有，本仓库仅用于个人学习与学术研究。
