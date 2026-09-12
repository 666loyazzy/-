# Other Knowledge Paper Index

The following 16 papers were moved out of the strict edge–cloud branch because their main execution path is datacenter-only or device-only.

| # | Paper | Why it is background rather than strict edge–cloud collaboration |
|---:|---|---|
| 1 | Splitwise | Datacenter Prefill/Decode phase splitting; no end/edge–cloud boundary. |
| 2 | Helix | Heterogeneous datacenter GPU placement and network scheduling. |
| 3 | TPLA | Datacenter disaggregated Prefill/Decode tensor parallelism. |
| 4 | MuxWise | Datacenter Prefill/Decode resource multiplexing. |
| 5 | Past-Future Scheduler | Datacenter SLA-aware LLM request scheduling. |
| 6 | QoServe / Niyama | Datacenter inference co-scheduling and isolation. |
| 7 | Shift Parallelism | Datacenter parallelism switching for dynamic workloads. |
| 8 | XY-Serve | Production datacenter LLM serving. |
| 9 | Bullet | Datacenter spatial-temporal GPU orchestration. |
| 10 | DynamoLLM | Datacenter inference-cluster design and reconfiguration. |
| 11 | POD-Attention | GPU-kernel-level Prefill/Decode overlap. |
| 12 | SwiftSpec | Disaggregated speculative decoding inside server infrastructure. |
| 13 | vAttention | Datacenter virtual-memory management for KV cache. |
| 14 | AQUA | Memory offloading inside scale-up GPU domains. |
| 15 | Kelle | Edge-side KV/eDRAM design without cloud-side collaborative execution. |
| 16 | llm.npu | On-device-only heterogeneous NPU inference. |

All files retain their original source/translation names so links remain easy to trace. DynoPipe is intentionally absent; it remains in the strict `edge-cloud-papers` branch.
