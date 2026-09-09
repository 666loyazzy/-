# 机器人与 ROS 2 论文选读 - 第 1 期

本期共 **12 篇**。每项均提供原文、纯中文嵌字版、中英双语版、规范引用和阅读提示。

## 1. 机器人算法与 Python 实现

**PythonRobotics: a Python code collection of robotics algorithms**  
Atsushi Sakai, Daniel Ingram, Joseph Dinius, Karan Chawla, Antonin Raffin, Alexis Paques（2018，8 页）

- [原文 PDF](papers/original/PythonRobotics_arXiv1808.10703v3.pdf)
- [纯中文嵌字版](papers/translated/PythonRobotics_arXiv1808.10703v3-mono.pdf)
- [中英双语版](papers/translated/PythonRobotics_arXiv1808.10703v3-dual.pdf)
- [arXiv 原文与引用](https://arxiv.org/abs/1808.10703)
- [阅读提示](notes/PythonRobotics.md)

先读引言和算法示例，选一个定位或规划动画，解释输入、输出与参数变化。

## 2. ROS 2 的设计与系统架构

**Robot Operating System 2: Design, Architecture, and Uses In The Wild**  
Steve Macenski, Tully Foote, Brian Gerkey, Chris Lalancette, William Woodall  
Science Robotics, 2022, 7(66): eabm6074. DOI: `10.1126/scirobotics.abm6074`（13 页）

- [原文 PDF](papers/original/ROS2_Design_Architecture_Uses_arXiv2211.07752v1.pdf)
- [纯中文嵌字版](papers/translated/ROS2_Design_Architecture_Uses_arXiv2211.07752v1-mono.pdf)
- [中英双语版](papers/translated/ROS2_Design_Architecture_Uses_arXiv2211.07752v1-dual.pdf)
- [arXiv 原文与引用](https://arxiv.org/abs/2211.07752)
- [阅读提示](notes/ROS2-Architecture.md)

先看架构图、通信设计与应用案例，联系课堂中的节点、话题和 QoS。

## 3. 移动机器人传感器综述

**A Review of Sensing Technologies for Indoor Autonomous Mobile Robots**  
Yu Liu, Shuting Wang, Yuanlong Xie, Tifan Xiong, Mingyuan Wu  
Sensors, 2024, 24(4): 1222. DOI: `10.3390/s24041222`（31 页）

- [原文 PDF](papers/original/Indoor_Mobile_Robot_Sensing_Review_Sensors2024.pdf)
- [纯中文嵌字版](papers/translated/Indoor_Mobile_Robot_Sensing_Review_Sensors2024-mono.pdf)
- [中英双语版](papers/translated/Indoor_Mobile_Robot_Sensing_Review_Sensors2024-dual.pdf)
- [期刊原文与引用](https://www.mdpi.com/1424-8220/24/4/1222)
- [阅读提示](notes/Sensing-Review.md)

先读单传感器部分，比较雷达、相机、IMU 与编码器的测量内容和局限；融合部分可后读。

## 4. 二维激光建图与 SLAM Toolbox

**SLAM Toolbox: SLAM for the dynamic world**  
Steve Macenski, Ivona Jambrecic  
Journal of Open Source Software, 2021, 6(61): 2783. DOI: `10.21105/joss.02783`（7 页）

- [原文 PDF](papers/original/SLAM_Toolbox_JOSS2021.pdf)
- [纯中文嵌字版](papers/translated/SLAM_Toolbox_JOSS2021-mono.pdf)
- [中英双语版](papers/translated/SLAM_Toolbox_JOSS2021-dual.pdf)
- [JOSS 原文与引用](https://joss.theoj.org/papers/10.21105/joss.02783)
- [阅读提示](notes/SLAM-Toolbox.md)

先理解地图更新、定位与多次建图的用途，再与课堂建图实验对应。

## 5. 移动机器人路径规划综述

**Path Planning for Autonomous Mobile Robots: A Review**  
J. Ricardo Sánchez-Ibáñez, Carlos J. Pérez-del-Pulgar, Alfonso García-Cerezo  
Sensors, 2021, 21(23): 7898. DOI: `10.3390/s21237898`（29 页）

- [原文 PDF](papers/original/Mobile_Robot_Path_Planning_Review_Sensors2021.pdf)
- [纯中文嵌字版](papers/translated/Mobile_Robot_Path_Planning_Review_Sensors2021-mono.pdf)
- [中英双语版](papers/translated/Mobile_Robot_Path_Planning_Review_Sensors2021-dual.pdf)
- [期刊原文与引用](https://www.mdpi.com/1424-8220/21/23/7898)
- [阅读提示](notes/Path-Planning-Review.md)

先看分类与示意图，区分全局和局部规划，再选搜索法或采样法做比较，不必一次读完。

## 6. 点云与三维数据处理

**Open3D: A Modern Library for 3D Data Processing**  
Qian-Yi Zhou, Jaesik Park, Vladlen Koltun（2018，6 页）

- [原文 PDF](papers/original/Open3D_arXiv1801.09847v1.pdf)
- [纯中文嵌字版](papers/translated/Open3D_arXiv1801.09847v1-mono.pdf)
- [中英双语版](papers/translated/Open3D_arXiv1801.09847v1-dual.pdf)
- [arXiv 原文与引用](https://arxiv.org/abs/1801.09847)
- [阅读提示](notes/Open3D.md)

先看数据表示与处理流程，理解点云、下采样和配准；可配合 Python 示例阅读。

## 7. Nav2 导航系统与行为树

**The Marathon 2: A Navigation System**  
Steve Macenski, Francisco Martín, Ruffin White, Jonatan Ginés Clavero  
IROS 2020: 2718-2725. DOI: `10.1109/IROS45743.2020.9341207`（8 页）

- [原文 PDF](papers/original/Marathon2_Navigation_System_arXiv2003.00368v2.pdf)
- [纯中文嵌字版](papers/translated/Marathon2_Navigation_System_arXiv2003.00368v2-mono.pdf)
- [中英双语版](papers/translated/Marathon2_Navigation_System_arXiv2003.00368v2-dual.pdf)
- [arXiv 原文与引用](https://arxiv.org/abs/2003.00368)
- [阅读提示](notes/Marathon2-Nav2.md)

先看系统架构和实验，说明规划、控制与恢复行为如何配合；它是架构论文，不是 Humble 安装教程。

## 8. 路径跟踪与速度调节

**Regulated Pure Pursuit for Robot Path Tracking**  
Steve Macenski, Shrijit Singh, Francisco Martín, Jonatan Ginés  
Autonomous Robots, 2023, 47(6): 685-694. DOI: `10.1007/s10514-023-10097-6`（11 页）

- [原文 PDF](papers/original/Regulated_Pure_Pursuit_arXiv2305.20026v1.pdf)
- [纯中文嵌字版](papers/translated/Regulated_Pure_Pursuit_arXiv2305.20026v1-mono.pdf)
- [中英双语版](papers/translated/Regulated_Pure_Pursuit_arXiv2305.20026v1-dual.pdf)
- [arXiv 原文与引用](https://arxiv.org/abs/2305.20026)
- [阅读提示](notes/Regulated-Pure-Pursuit.md)

结合示意图理解前视点与曲率，再看速度调节和实验对比；需要基本移动机器人运动学。

## 9. 卡尔曼滤波的逐步推导

**A Step by Step Mathematical Derivation and Tutorial on Kalman Filters**  
Hamed Masnadi-Shirazi, Alireza Masnadi-Shirazi, Mohammad-Amir Dastgheib（2019，32 页）

- [原文 PDF](papers/original/Kalman_Filter_Tutorial_arXiv1910.03558v1.pdf)
- [纯中文嵌字版](papers/translated/Kalman_Filter_Tutorial_arXiv1910.03558v1-mono.pdf)
- [中英双语版](papers/translated/Kalman_Filter_Tutorial_arXiv1910.03558v1-dual.pdf)
- [arXiv 原文与引用](https://arxiv.org/abs/1910.03558)
- [阅读提示](notes/Kalman-Filter-Tutorial.md)

先理解预测与校正，再阅读状态模型和递推公式。需要线性代数与概率基础，完整证明留作进阶。

## 10. 激光里程计与 ICP 配准

**KISS-ICP: In Defense of Point-to-Point ICP - Simple, Accurate, and Robust Registration If Done the Right Way**  
Ignacio Vizzo, Tiziano Guadagnino, Benedikt Mersch, Louis Wiesmann, Jens Behley, Cyrill Stachniss  
IEEE Robotics and Automation Letters, 2023, 8(2): 1029-1036. DOI: `10.1109/LRA.2023.3236571`（8 页）

- [原文 PDF](papers/original/KISS-ICP_RAL2023.pdf)
- [纯中文嵌字版](papers/translated/KISS-ICP_RAL2023-mono.pdf)
- [中英双语版](papers/translated/KISS-ICP_RAL2023-dual.pdf)
- [arXiv 原文与引用](https://arxiv.org/abs/2209.15397)
- [阅读提示](notes/KISS-ICP.md)

先看流程图和实验，说明相邻点云如何通过刚体变换估计运动；先具备刚体变换、最近邻搜索与最小二乘基础。

## 11. 视觉 SLAM 系统

**ORB-SLAM2: an Open-Source SLAM System for Monocular, Stereo and RGB-D Cameras**  
Raúl Mur-Artal, Juan D. Tardós  
IEEE Transactions on Robotics, 2017, 33(5): 1255-1262. DOI: `10.1109/TRO.2017.2705103`（9 页）

- [原文 PDF（含 1 页版权封面）](papers/original/ORB-SLAM2_TRO2017_arXiv1610.06475v1.pdf)
- [纯中文嵌字版（8 页正文）](papers/translated/ORB-SLAM2_TRO2017_arXiv1610.06475v1-mono.pdf)
- [中英双语版（8 页正文）](papers/translated/ORB-SLAM2_TRO2017_arXiv1610.06475v1-dual.pdf)
- [arXiv 原文与引用](https://arxiv.org/abs/1610.06475)
- [阅读提示](notes/ORB-SLAM2.md)

先看系统框架，区分 Tracking、Local Mapping、Loop Closing 三个线程。先修知识：相机模型、特征匹配、位姿估计和基本优化。

## 12. SLAM 的整体知识框架

**Past, Present, and Future of Simultaneous Localization and Mapping: Towards the Robust-Perception Age**  
Cesar Cadena, Luca Carlone, Henry Carrillo, Yasir Latif, Davide Scaramuzza, José Neira, Ian Reid, John J. Leonard  
IEEE Transactions on Robotics, 2016, 32(6): 1309-1332. DOI: `10.1109/TRO.2016.2624754`（作者定稿 24 页）

- [原文 PDF](papers/original/SLAM-Robust-Perception_TRO2016.pdf)
- [纯中文嵌字版](papers/translated/SLAM-Robust-Perception_TRO2016-mono.pdf)
- [中英双语版](papers/translated/SLAM-Robust-Perception_TRO2016-dual.pdf)
- [IEEE 原文与引用](https://doi.org/10.1109/TRO.2016.2624754)
- [阅读提示](notes/SLAM-Robust-Perception.md)

作为课程后半段的知识地图，先读引言、系统划分、鲁棒性与开放问题；不要求首次阅读掌握全部数学推导。
