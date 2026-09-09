# PDF 来源与校验

更新时间：2026-09-09。当前共 **12 篇原文、12 份纯中文嵌字版、12 份中英双语版**。

| # | 论文 | 公共来源 | 原文页数 | 中文页数 | 双语页数 |
|---:|---|---|---:|---:|---:|
| 1 | PythonRobotics | [arXiv:1808.10703](https://arxiv.org/abs/1808.10703) | 8 | 8 | 16 |
| 2 | Robot Operating System 2 | [arXiv:2211.07752](https://arxiv.org/abs/2211.07752) | 13 | 13 | 26 |
| 3 | Indoor Mobile Robot Sensing Review | [Sensors 24(4), 1222](https://www.mdpi.com/1424-8220/24/4/1222) | 31 | 31 | 62 |
| 4 | SLAM Toolbox | [JOSS 02783](https://joss.theoj.org/papers/10.21105/joss.02783) | 7 | 7 | 14 |
| 5 | Mobile Robot Path Planning Review | [Sensors 21(23), 7898](https://www.mdpi.com/1424-8220/21/23/7898) | 29 | 29 | 58 |
| 6 | Open3D | [arXiv:1801.09847](https://arxiv.org/abs/1801.09847) | 6 | 6 | 12 |
| 7 | The Marathon 2 | [arXiv:2003.00368](https://arxiv.org/abs/2003.00368) | 8 | 8 | 16 |
| 8 | Regulated Pure Pursuit | [arXiv:2305.20026](https://arxiv.org/abs/2305.20026) | 11 | 11 | 22 |
| 9 | Kalman Filter Tutorial | [arXiv:1910.03558](https://arxiv.org/abs/1910.03558) | 32 | 32 | 64 |
| 10 | KISS-ICP | [University of Bonn 作者 PDF](https://www.ipb.uni-bonn.de/pdfs/vizzo2023ral.pdf) | 8 | 8 | 16 |
| 11 | ORB-SLAM2 | [arXiv:1610.06475](https://arxiv.org/abs/1610.06475) | 9 | 8 | 16 |
| 12 | SLAM Robust-Perception Survey | [University of Zurich 作者 PDF](https://rpg.ifi.uzh.ch/docs/TRO16_cadena.pdf) | 24 | 24 | 48 |

双语版采用“英文原页 + 中文译页”逐页配对。ORB-SLAM2 原文第 1 页为版权封面，译文略去该页，因此其中文版本为 8 页、双语版本为 16 页。

## 目录

- [`original/`](original/) - 12 篇原文 PDF
- [`translated/`](translated/) - 纯中文与中英双语 PDF
- [`SHA256SUMS.txt`](SHA256SUMS.txt) - 36 个 PDF 的 SHA-256 校验值

## 翻译与检查

- 工具：PDFMathTranslate / `pdf2zh`
- 语言：English -> Chinese
- 服务：Google Translate
- 检查：所有 PDF 均可由 Poppler 打开；中文版本页数与正文一致；双语版本页数为中文版本的两倍；新增译文完成逐页缩略图和双语首/中/尾页渲染检查。

机器翻译仅用于辅助阅读；论文数据、公式、引用与结论请以原文为准。著作权归原作者及出版机构所有。
