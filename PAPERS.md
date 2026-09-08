# Robotics / SLAM Paper Index

## 1. 激光里程计与 ICP 配准

**KISS-ICP: In Defense of Point-to-Point ICP - Simple, Accurate, and Robust Registration If Done the Right Way**  
Ignacio Vizzo, Tiziano Guadagnino, Benedikt Mersch, Louis Wiesmann, Jens Behley, Cyrill Stachniss  
IEEE Robotics and Automation Letters, 2023, 8(2): 1029-1036. DOI: `10.1109/LRA.2023.3236571`

- [官方原文 PDF](papers/original/KISS-ICP_RAL2023.pdf)
- [纯中文嵌字版](papers/translated/KISS-ICP_RAL2023-mono.pdf)
- [中英双语版](papers/translated/KISS-ICP_RAL2023-dual.pdf)
- [阅读提示](notes/KISS-ICP.md)

推荐先看方法流程图和实验，回答“相邻两帧点云如何通过刚体变换估计运动”。先修知识：刚体变换、最近邻搜索和最小二乘。

## 2. 视觉 SLAM 系统

**ORB-SLAM2: an Open-Source SLAM System for Monocular, Stereo and RGB-D Cameras**  
Raúl Mur-Artal, Juan D. Tardós  
IEEE Transactions on Robotics, 2017, 33(5): 1255-1262. DOI: `10.1109/TRO.2017.2705103`

- [官方原文 PDF（arXiv，含 1 页版权封面）](papers/original/ORB-SLAM2_TRO2017_arXiv1610.06475v1.pdf)
- [纯中文嵌字版（8 页正文）](papers/translated/ORB-SLAM2_TRO2017_arXiv1610.06475v1-mono.pdf)
- [中英双语版（8 页正文）](papers/translated/ORB-SLAM2_TRO2017_arXiv1610.06475v1-dual.pdf)
- [阅读提示](notes/ORB-SLAM2.md)

推荐先看系统框架，区分 Tracking、Local Mapping、Loop Closing 三个线程。先修知识：针孔相机模型、ORB 特征匹配、位姿估计和基本非线性优化。

## 3. SLAM 的整体知识框架

**Past, Present, and Future of Simultaneous Localization and Mapping: Towards the Robust-Perception Age**  
Cesar Cadena, Luca Carlone, Henry Carrillo, Yasir Latif, Davide Scaramuzza, José Neira, Ian Reid, John J. Leonard  
IEEE Transactions on Robotics, 2016, 32(6): 1309-1332. DOI: `10.1109/TRO.2016.2624754`

- [作者主页正式定稿 PDF](papers/original/SLAM-Robust-Perception_TRO2016.pdf)
- [纯中文嵌字版](papers/translated/SLAM-Robust-Perception_TRO2016-mono.pdf)
- [中英双语版](papers/translated/SLAM-Robust-Perception_TRO2016-dual.pdf)
- [阅读提示](notes/SLAM-Robust-Perception.md)

推荐作为课程后半段的知识地图，先读引言、SLAM 系统划分、鲁棒性与开放问题。作者主页的 IEEE 定稿为 24 页（期刊页码 1309-1332），部分检索卡片标作 25 页，仓库以实际 PDF 为准。
