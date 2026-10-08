# 论文分类索引

当前按主索引统计共 **48 篇不重复论文**：严格边云协同 20 篇、其它辅助知识 16 篇、机器人与 ROS 2 论文 12 篇。

## A. 边云协同独立分支（20）

完整论文清单、原文、中文与双语译文、来源记录和研究笔记统一保存在 [`edge-cloud-papers`](https://github.com/666loyazzy/-/tree/edge-cloud-papers) 分支。

[打开完整论文清单](https://github.com/666loyazzy/-/blob/edge-cloud-papers/PAPERS.md)

## B. 其它辅助知识（16）

1. **Splitwise** — 数据中心 Prefill/Decode 阶段拆分
2. **Helix** — 异构数据中心 GPU 放置与网络调度
3. **TPLA** — 数据中心解耦式 Prefill/Decode 张量并行
4. **MuxWise** — 数据中心 Prefill/Decode 资源复用
5. **Past-Future Scheduler** — 数据中心 SLA 感知请求调度
6. **QoServe / Niyama** — 数据中心推理协同调度与隔离
7. **Shift Parallelism** — 数据中心动态工作负载并行策略切换
8. **XY-Serve** — 生产环境数据中心 LLM serving
9. **Bullet** — 数据中心 GPU 时空编排
10. **DynamoLLM** — 数据中心推理集群设计与重配置
11. **POD-Attention** — GPU 内核级 Prefill/Decode 重叠
12. **SwiftSpec** — 服务器基础设施内的解耦式推测解码
13. **vAttention** — 数据中心 KV cache 虚拟内存管理
14. **AQUA** — Scale-up GPU 域内存卸载
15. **Kelle** — 无云侧协同执行的边缘 KV/eDRAM 设计
16. **llm.npu** — 纯端侧异构 NPU 推理

[查看辅助知识分支](https://github.com/666loyazzy/-/blob/other-knowledge/PAPERS.md)

## C. 机器人与 ROS 2（12）

1. **PythonRobotics: a Python code collection of robotics algorithms** — 2018
2. **Robot Operating System 2: Design, Architecture, and Uses In The Wild** — 2022
3. **A Review of Sensing Technologies for Indoor Autonomous Mobile Robots** — 2024
4. **SLAM Toolbox: SLAM for the dynamic world** — 2021
5. **Path Planning for Autonomous Mobile Robots: A Review** — 2021
6. **Open3D: A Modern Library for 3D Data Processing** — 2018
7. **The Marathon 2: A Navigation System** — 2020
8. **Regulated Pure Pursuit for Robot Path Tracking** — 2023
9. **A Step by Step Mathematical Derivation and Tutorial on Kalman Filters** — 2019
10. **KISS-ICP: In Defense of Point-to-Point ICP — Simple, Accurate, and Robust Registration If Done the Right Way** — 2023
11. **ORB-SLAM2: an Open-Source SLAM System for Monocular, Stereo and RGB-D Cameras** — 2017
12. **Past, Present, and Future of Simultaneous Localization and Mapping: Towards the Robust-Perception Age** — 2016

[查看机器人分支](https://github.com/666loyazzy/-/blob/robotics-papers/PAPERS.md)

## 计数与维护规则

- 同一篇论文的原文、中文版和双语版只计为 1 篇。
- `main` 保留分类索引和现有辅助知识文件；边云协同资料统一在独立分支维护。
- 边云协同完整清单、PDF 与研究资料统一由 `edge-cloud-papers` 分支维护。
- `other-knowledge` 和 `robotics-papers` 的现有资料保持独立，不因纯边云集合替换而改动。
