# Awesome Robotics & ROS 2 Papers

机器人与 ROS 2 论文选读仓库。当前收录课程“论文选读·第 1 期”的 **12 篇论文**，覆盖算法实现、ROS 2 架构、传感器、点云、定位建图、路径规划、导航控制和卡尔曼滤波。

每篇论文统一整理：原文 PDF、纯中文嵌字版、中英双语版、BibTeX 引用和阅读提示。

## 分支导航

- [`main`](https://github.com/666loyazzy/-/tree/main) - 全仓库总入口与跨方向论文清单
- [`edge-cloud-papers`](https://github.com/666loyazzy/-/tree/edge-cloud-papers) - DynoPipe / 边云协同论文库
- [`robotics-papers`](https://github.com/666loyazzy/-/tree/robotics-papers) - 机器人与 ROS 2 论文库（当前分支）

## 第 1 期论文清单

| # | 主题 | 论文 | 年份 |
|---:|---|---|---:|
| 1 | 机器人算法与 Python 实现 | PythonRobotics | 2018 |
| 2 | ROS 2 的设计与系统架构 | Robot Operating System 2 | 2022 |
| 3 | 移动机器人传感器综述 | A Review of Sensing Technologies for Indoor Autonomous Mobile Robots | 2024 |
| 4 | 二维激光建图 | SLAM Toolbox | 2021 |
| 5 | 移动机器人路径规划综述 | Path Planning for Autonomous Mobile Robots | 2021 |
| 6 | 点云与三维数据处理 | Open3D | 2018 |
| 7 | Nav2 与行为树 | The Marathon 2 | 2020 |
| 8 | 路径跟踪与速度调节 | Regulated Pure Pursuit | 2023 |
| 9 | 卡尔曼滤波推导 | A Step by Step Mathematical Derivation and Tutorial on Kalman Filters | 2019 |
| 10 | 激光里程计与 ICP | KISS-ICP | 2023 |
| 11 | 视觉 SLAM 系统 | ORB-SLAM2 | 2017 |
| 12 | SLAM 整体知识框架 | Past, Present, and Future of SLAM | 2016 |

## 建议阅读路线

无需按编号顺序读。初学路线可按以下顺序：

1. **PythonRobotics**：先用动画建立定位、规划和控制的直觉。
2. **ROS 2 → SLAM Toolbox → Marathon 2**：把节点、话题、QoS、建图和 Nav2 串成系统。
3. **Open3D → KISS-ICP**：理解点云处理和相邻帧配准。
4. **路径规划综述 → Regulated Pure Pursuit**：区分全局规划与局部跟踪。
5. **Kalman Filters → ORB-SLAM2**：补状态估计和视觉 SLAM。
6. **传感器综述 → SLAM 综述**：最后建立完整知识地图。

## 仓库文件

- [`PAPERS.md`](PAPERS.md) - 12 篇论文的完整索引、来源、译文和阅读提示
- [`references.bib`](references.bib) - 可直接用于 Overleaf 的 BibTeX
- [`papers/original/`](papers/original/) - 原文 PDF
- [`papers/translated/`](papers/translated/) - 纯中文嵌字版与中英双语版
- [`papers/README.md`](papers/README.md) - PDF 来源、页数、校验值与翻译状态
- [`notes/`](notes/) - 每篇论文的阅读抓手和先修知识

## 翻译说明

译文使用 PDFMathTranslate / `pdf2zh`（英文到中文、Google 翻译服务）生成，尽量保留公式、图表和原版布局。仓库对输出 PDF 进行可打开性、页数与页面渲染检查。

PDF 著作权归原作者及出版机构所有，本仓库仅用于个人学习与学术研究。
