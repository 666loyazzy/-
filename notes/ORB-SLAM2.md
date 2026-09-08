# ORB-SLAM2 reading guide

## 先回答的问题

视觉 SLAM 为什么不能只靠逐帧特征匹配，而需要跟踪、局部建图、回环检测与全局优化协同工作？

## 阅读抓手

1. 先看系统框架，明确三个主线程：Tracking、Local Mapping、Loop Closing。
2. Tracking 负责当前帧定位并决定是否插入关键帧；Local Mapping 扩充和优化局部地图；Loop Closing 识别曾到过的位置并消除累计漂移。
3. 单目、双目、RGB-D 的共同部分是特征与图优化，关键区别是深度和尺度能否直接观测。
4. 重点理解 ORB 特征、共视图、关键帧、地图点、Bundle Adjustment、BoW 回环词袋之间的连接关系。

## 先修知识

针孔相机模型、坐标变换、ORB 特征与描述子、PnP、三角化、Bundle Adjustment。
