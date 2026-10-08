# 论文阅读与研究资料库

本仓库按独立分支整理严格端/边—云协同 LLM、其它边云与 LLM 系统辅助知识、机器人与 ROS 2。边云协同论文、完整清单和研究资料统一保存在 `edge-cloud-papers` 分支；`main` 保留分支导航、辅助知识资料和机器人索引。

## 分支导航

| 分支 | 内容 | 论文数 | 说明 |
|---|---|---:|---|
| [`edge-cloud-papers`](https://github.com/666loyazzy/-/tree/edge-cloud-papers) | 严格端/边—云协同 LLM 推理 | 20 | 唯一有效的严格边云集合 |
| [`other-knowledge`](https://github.com/666loyazzy/-/tree/other-knowledge) | LLM serving、端侧推理、数据中心调度与历史机制等辅助知识 | 16 | 原有背景知识保持不变 |
| [`robotics-papers`](https://github.com/666loyazzy/-/tree/robotics-papers) | 移动机器人、ROS 2、传感器、规划、控制、定位与 SLAM | 12 | 原有机器人论文保持不变 |

按主索引统计，共 **48 篇不重复论文**：严格边云协同 20 篇、辅助知识 16 篇、机器人与 ROS 2 论文 12 篇。分类索引见 [`PAPERS.md`](PAPERS.md)，各主题完整清单见对应分支。

## 其它辅助知识（16）

`main` 中现有的辅助资料保持不变，包括 Splitwise（数据中心 Prefill/Decode 拆分）、Helix、TPLA、MuxWise、Past-Future Scheduler、QoServe/Niyama、Shift Parallelism、XY-Serve、Bullet、DynamoLLM、POD-Attention、SwiftSpec、vAttention、AQUA、Kelle 和 llm.npu。

这些论文用于理解数据中心 serving、调度、推测解码、KV-cache/内存、端侧推理与硬件机制，不计入严格边云协同 20 篇。文件索引见 [`papers/README.md`](papers/README.md)，主题分支见 [`other-knowledge`](https://github.com/666loyazzy/-/tree/other-knowledge)。

## 机器人与 ROS 2（12）

机器人资料保持原样，覆盖 PythonRobotics、ROS 2 架构、移动机器人传感、SLAM Toolbox、路径规划、Open3D、Navigation、Pure Pursuit、Kalman Filter、KISS-ICP、ORB-SLAM2 和 SLAM 综述。

完整清单见 [`PAPERS.md`](PAPERS.md)，论文文件见 [`robotics-papers`](https://github.com/666loyazzy/-/tree/robotics-papers)。

同一篇论文的英文原文、中文单语版和中英双语版只计为 1 篇。PDF 著作权归原作者及出版机构所有，本仓库内容仅用于个人学习与学术研究。
