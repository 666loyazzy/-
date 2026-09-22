# 辅助知识论文文件

本目录只保留 16 篇边云与 LLM 系统辅助知识，不属于严格端/边—云协同 LLM 20 篇集合。

- `original/`：公开原文或预印本 PDF。
- `translated/`：对应的中文单语版与中英双语版。
- 严格边云论文统一放在 [`edge-cloud-papers`](https://github.com/666loyazzy/-/tree/edge-cloud-papers) 分支。

## 文件清单

| # | 论文 | 本地原文 | 说明 |
|---:|---|---|---|
| 1 | Splitwise | `original/Splitwise_ISCA24_arXiv2311.18677v2.pdf` | 数据中心 Prefill/Decode 阶段拆分 |
| 2 | Helix | `original/Helix_ASPLOS25_arXiv2406.01566v2.pdf` | 异构数据中心 GPU 放置与网络调度 |
| 3 | TPLA | `original/TPLA_ASPLOS26_arXiv2508.15881v2.pdf` | 解耦式 Prefill/Decode 张量并行 |
| 4 | MuxWise | `original/MuxWise_ASPLOS26_arXiv2504.14489v3.pdf` | Prefill/Decode 资源复用 |
| 5 | Past-Future Scheduler | `original/Past-Future-Scheduler_ASPLOS25_arXiv2507.10150v1.pdf` | SLA 感知请求调度 |
| 6 | QoServe / Niyama | `original/QoServe_ASPLOS26_preprint-Niyama-arXiv2503.22562v1.pdf` | 推理调度与隔离 |
| 7 | Shift Parallelism | `original/Shift-Parallelism_ASPLOS26_arXiv2509.16495v2.pdf` | 动态并行策略切换 |
| 8 | XY-Serve | `original/XY-Serve_ASPLOS26_preprint-arXiv2412.18106v1.pdf` | 生产环境 LLM serving |
| 9 | Bullet | `original/Bullet_ASPLOS26_arXiv2504.19516v4.pdf` | GPU 时空编排 |
| 10 | DynamoLLM | `original/DynamoLLM_HPCA25_arXiv2408.00741v1.pdf` | 推理集群设计与重配置 |
| 11 | POD-Attention | `original/POD-Attention_ASPLOS25_arXiv2410.18038v2.pdf` | Prefill/Decode 内核重叠 |
| 12 | SwiftSpec | `original/SwiftSpec_ASPLOS26_arXiv2506.11309v1.pdf` | 服务器基础设施内推测解码 |
| 13 | vAttention | `original/vAttention_ASPLOS25_arXiv2405.04437v3.pdf` | KV-cache 虚拟内存管理 |
| 14 | AQUA | `original/AQUA_ASPLOS25_arXiv2407.21255v3.pdf` | GPU 域内存卸载 |
| 15 | Kelle | `original/Kelle_MICRO25_arXiv2510.16040v1.pdf` | 边缘 KV/eDRAM 设计 |
| 16 | llm.npu | `original/llm.npu_ASPLOS25_arXiv2407.05858v2.pdf` | 纯端侧异构 NPU 推理 |

翻译文件见 [`translated/README.md`](translated/README.md)。PDF 著作权归原作者及出版机构所有，本目录仅用于个人学习与学术研究。
