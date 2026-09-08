# Awesome Robotics Papers - SLAM Starter Track

面向机器人定位与建图入门的精简论文库。本分支只收录当前学习路线中的三篇核心论文，并同时保存官方原文、纯中文嵌字版、中英双语版、规范引用和阅读提示。

## Repository branches

- [`main`](https://github.com/666loyazzy/-/tree/main) - 仓库入口与原始主线
- [`edge-cloud-papers`](https://github.com/666loyazzy/-/tree/edge-cloud-papers) - DynoPipe / 边云协同论文库
- [`robotics-papers`](https://github.com/666loyazzy/-/tree/robotics-papers) - 机器人与 SLAM 论文库（当前分支）

## Reading order

1. **KISS-ICP**：从相邻 LiDAR 点云配准理解“如何由两帧观测估计机器人运动”。先看流程图与实验，再看点到点 ICP、鲁棒核、运动补偿和自适应阈值。
2. **ORB-SLAM2**：从完整视觉 SLAM 系统理解跟踪、局部建图和回环三个并行模块，以及地图复用与重定位。
3. **SLAM: Past, Present, and Future**：建立 SLAM 的整体知识地图，重点读引言、系统划分、鲁棒性与开放挑战，不要求首次阅读掌握全部推导。

## Files

- [`PAPERS.md`](PAPERS.md) - 论文索引、下载入口和推荐读法
- [`references.bib`](references.bib) - 可直接用于 LaTeX 的 BibTeX 引用
- [`papers/original/`](papers/original/) - 官方作者主页或 arXiv 原文
- [`papers/translated/`](papers/translated/) - PDFMathTranslate 生成的纯中文与中英双语版
- [`papers/README.md`](papers/README.md) - 来源、页数、文件校验值和翻译说明
- [`notes/`](notes/) - 三篇论文的阅读抓手与先修知识

## Translation note

译文使用 `pdf2zh v1.9.11`（PDFMathTranslate，英文到中文）生成，保留公式、图表和原版双栏布局，并完成逐页缩略图检查。ORB-SLAM2 的 9 页 arXiv 文件第 1 页仅为版权与收录信息，旋转文字会干扰版面识别，因此原文完整保留 9 页，译文只处理后 8 页论文正文。

PDF 的著作权归原作者及出版机构所有，本仓库仅用于个人学习与学术研究。
