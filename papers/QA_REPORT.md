# PDF 翻译验收报告

验收对象：`edge-cloud-papers` 分支中的 20 篇严格边云协同论文；每篇均包含英文原文、中文单语版（`-mono.pdf`）和中英双语版（`-dual.pdf`）。

## 验收标准

- 原文 PDF 可由 `pdfinfo` 正常解析。
- 单语版页数与原文一致；双语版页数为原文的两倍（PDFMathTranslate 的逐页中英对照输出方式）。
- 单语版可提取中文文本，且不存在已知误译“法学硕士”“多模态法学硕士”“多模式法学硕士”。
- 中文字体为嵌入式 Source Han Serif CN；`pdffonts` 的 `emb` 字段必须为 `yes`。
- 40 份译文逐页渲染检查必须全部成功；本批次共检查 780 个译文页面。
- 对标题页、正文中间页、参考文献页及双语页进行人工抽查，确认无中文豆腐块或字体渲染失败。原论文自带的可点击交叉引用边框不视为字体缺字。

## AI 术语策略

- 保留业界通行缩写：LLM、SLM、DNN、MoE、KV cache、TTFT、TPOT 等，不强行扩写或创造译名。
- 采用稳定中文术语：大语言模型、边云协同推理、模型切分、计算卸载、推测解码、流水线并行、协同推理、特征压缩。
- 术语修正采用 PDF 真正删改：先删除错误文字对象，再嵌入 Source Han Serif CN 写入正确中文；不是用白色方块遮盖。

## 逐篇结果

| 论文文件 | 原文页数 | 单语页数 | 双语页数 | 中文字体嵌入 | 坏术语残留 | 全页渲染 |
|---|---:|---:|---:|---|---:|---|
| AceSpec_arXiv2609.02514 | 10 | 10 | 20 | PASS | 0 | PASS |
| AppealNet_DAC21_arXiv2105.04104 | 6 | 6 | 12 | PASS | 0 | PASS |
| BottleNetPlusPlus_ICCW20_arXiv1910.14315 | 6 | 6 | 12 | PASS | 0 | PASS |
| CE-CoLLM_arXiv2411.02829 | 8 | 8 | 16 | PASS | 0 | PASS |
| CE-LSLM_arXiv2505.14085 | 14 | 14 | 28 | PASS | 0 | PASS |
| CLIO_MobiCom20 | 12 | 12 | 24 | PASS | 0 | PASS |
| DDNN_ICDCS17_arXiv1709.01921 | 12 | 12 | 24 | PASS | 0 | PASS |
| DynO_TECS22_arXiv2104.09949 | 24 | 24 | 48 | PASS | 0 | PASS |
| DynoPipe_ISCA26 | 16 | 16 | 32 | PASS | 0 | PASS |
| EdgeCloud_SLM_LLM_Survey_arXiv2507.16731 | 36 | 36 | 72 | PASS | 0 | PASS |
| EdgeShard_arXiv2405.14371 | 11 | 11 | 22 | PASS | 0 | PASS |
| Edgent_SEC18_arXiv1806.07840 | 10 | 10 | 20 | PASS | 0 | PASS |
| HAT_arXiv2503.18989 | 13 | 13 | 26 | PASS | 0 | PASS |
| JointDNN_TMC21_arXiv1801.08618 | 12 | 12 | 24 | PASS | 0 | PASS |
| MoA-Off_arXiv2509.16995 | 5 | 5 | 10 | PASS | 0 | PASS |
| MultiTASC_arXiv2306.12830 | 6 | 6 | 12 | PASS | 0 | PASS |
| Neurosurgeon_ASPLOS17 | 15 | 15 | 30 | PASS | 0 | PASS |
| PrivacyAware_EdgeCloud_LLM_arXiv2607.13093 | 15 | 15 | 30 | PASS | 0 | PASS |
| SPINN_MobiCom20_arXiv2008.06402 | 14 | 14 | 28 | PASS | 0 | PASS |
| SplitLLM_arXiv2410.10759 | 15 | 15 | 30 | PASS | 0 | PASS |

结论：20 篇原文、20 份单语译文和 20 份双语译文均通过自动与人工验收。
