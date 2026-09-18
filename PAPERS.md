# Other Knowledge Paper Index

## A. 相邻的 LLM 系统知识（16 篇）

| # | Paper | 不进入严格边云 LLM 核心的原因 |
|---:|---|---|
| 1 | Splitwise (ISCA 2024) | 数据中心 Prefill/Decode 解耦，不跨端/边—云边界。 |
| 2 | Helix | 数据中心异构 GPU 放置与网络调度。 |
| 3 | TPLA | 数据中心解耦式 Prefill/Decode 张量并行。 |
| 4 | MuxWise | 数据中心 Prefill/Decode 资源复用。 |
| 5 | Past-Future Scheduler | 数据中心 SLA 感知请求调度。 |
| 6 | QoServe / Niyama | 数据中心推理协同调度与隔离。 |
| 7 | Shift Parallelism | 数据中心动态负载下切换并行方式。 |
| 8 | XY-Serve | 生产数据中心 LLM serving。 |
| 9 | Bullet | 数据中心 GPU 时空编排。 |
| 10 | DynamoLLM | 数据中心推理集群设计与重构。 |
| 11 | POD-Attention | GPU 内核层 Prefill/Decode 重叠。 |
| 12 | SwiftSpec | 服务器基础设施内的解耦推测解码。 |
| 13 | vAttention | 数据中心 KV cache 虚拟内存管理。 |
| 14 | AQUA | Scale-up GPU 域内存卸载。 |
| 15 | Kelle | 仅边侧 KV/eDRAM，无云侧协同执行。 |
| 16 | llm.npu | 纯端侧异构 NPU 推理。 |

## B. 旧 CNN/DNN 协同推理（迁入 9 篇）

| # | Paper | 迁移理由 |
|---:|---|---|
| 17 | Neurosurgeon | 经典云—移动边缘切分推理，但对象是 DNN/CNN，不是 LLM。 |
| 18 | Edgent | 设备—边缘 DNN 协同与早退，不是 LLM。 |
| 19 | JointDNN | 移动云 DNN 训练/推理切分，不是 LLM。 |
| 20 | DDNN | 云、边与端的分布式 DNN，不是 LLM。 |
| 21 | BottleNet++ | 设备—边缘 CNN 中间特征压缩，不是 LLM。 |
| 22 | SPINN | 设备—云渐进式神经网络推理，不是 LLM。 |
| 23 | CLIO | IoT—云深度学习流水线编译，不是 LLM。 |
| 24 | AppealNet | 边—云 DNN 推理架构，不是 LLM。 |
| 25 | MultiTASC | 消费边缘级联 DNN 调度，不是 LLM。 |

DynO 虽然也是非 LLM，但因用户明确要求作为 DynoPipe 的历史桥接例外，仍留在核心分支并单独标注。
