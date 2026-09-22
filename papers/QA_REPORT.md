# PDF 翻译验收报告

验收对象：`edge-cloud-papers` 分支中的严格边云协同论文清单。当前包含 20 篇英文原文、20 份中文单语嵌字版（`-mono.pdf`）和 20 份中英双语嵌字版（`-dual.pdf`）。

## 验收标准

- 20 份原文均可由 `pdfinfo` 正常解析，共 254 页。
- 每份单语版页数与原文一致，共 254 页。
- 双语版采用两种兼容的版式：新版 BabelDOC 输出为同页左右对照，页数等于原文；仓库中保留的历史译文为逐页顺排，页数为原文的两倍。因此每份双语版页数必须为原文页数或其两倍；当前共 418 页。
- 单语版均可提取中文文本；每份中文字符数均超过 100；未发现“法学硕士”“多模态法学硕士”“多模式法学硕士”“大型语言模式”“大型语言模块”等已知误译或翻译错误标记。
- `pdffonts` 检查确认中文 Source Han Serif CN 字体已嵌入（`emb=yes`，并且字符映射可用）。
- 40 份译文逐页使用 Poppler 渲染；实际 PNG 页数与 `pdfinfo` 页数完全一致，无渲染失败页。
- 人工抽查新版单语页、双语对照页、图表密集页和参考文献页；未发现中文豆腐块、空白页、裁切、字体渲染失败或翻译后布局溢出。原论文自带的绿色/红色引用边框保留，不属于字体缺字。

## AI 术语策略

- 保留业界通行缩写：LLM、MLLM、SLM、DNN、MoE、KV cache、TTFT、TPOT 等。
- 采用体系结构与系统领域常用术语：大语言模型、边云协同推理、模型切分、计算卸载、推测解码、流水线并行、协同推理、特征压缩、目标模型、草稿模型。
- 翻译只改写文字对象并嵌入中文字体，不使用白色遮盖块伪装修复。

## 逐篇结果

| 论文文件 | 原文页数 | 单语页数 | 双语页数 | 中文字体 | 坏术语 | 渲染 |
|---|---:|---:|---:|---|---:|---|
| AceSpec_arXiv2609.02514 | 10 | 10 | 20 | PASS | 0 | PASS |
| BatteryAwareSpec_ICPP26 | 11 | 11 | 11 | PASS | 0 | PASS |
| CE-CoLLM_arXiv2411.02829 | 8 | 8 | 16 | PASS | 0 | PASS |
| CE-LSLM_arXiv2505.14085 | 14 | 14 | 28 | PASS | 0 | PASS |
| CoGenesis_ACL24 | 18 | 18 | 18 | PASS | 0 | PASS |
| Crayon_ACL24_arXiv2406.07007 | 12 | 12 | 12 | PASS | 0 | PASS |
| DiSCo_FindingsACL25 | 19 | 19 | 19 | PASS | 0 | PASS |
| DivisionOfThoughts_WWW25_arXiv2502.04392 | 12 | 12 | 12 | PASS | 0 | PASS |
| DynO_TECS22_arXiv2104.09949 | 24 | 24 | 48 | PASS | 0 | PASS |
| DynoPipe_ISCA26 | 16 | 16 | 32 | PASS | 0 | PASS |
| EdgeShard_arXiv2405.14371 | 11 | 11 | 22 | PASS | 0 | PASS |
| EfficientDeployment_SOCC24 | 6 | 6 | 6 | PASS | 0 | PASS |
| FlexSpec_TMC26_arXiv2601.00644 | 12 | 12 | 12 | PASS | 0 | PASS |
| HAT_arXiv2503.18989 | 13 | 13 | 26 | PASS | 0 | PASS |
| MoA-Off_arXiv2509.16995 | 5 | 5 | 10 | PASS | 0 | PASS |
| PICE_arXiv2501.09367 | 12 | 12 | 24 | PASS | 0 | PASS |
| PrivacyAware_EdgeCloud_LLM_arXiv2607.13093 | 15 | 15 | 30 | PASS | 0 | PASS |
| SplitLLM_arXiv2410.10759 | 15 | 15 | 30 | PASS | 0 | PASS |
| Splitwise_UCC25_arXiv2512.23310 | 11 | 11 | 22 | PASS | 0 | PASS |
| Ygg_IWQoS26 | 10 | 10 | 20 | PASS | 0 | PASS |
| **合计** | **254** | **254** | **418** | **PASS** | **0** | **PASS** |

结论：当前工作区中的 20 篇原文、20 份中文单语版和 20 份中英双语版均通过自动检查与人工版式抽查。
