# DynoPipe-Direction Paper Index

Only papers directly relevant to **dynamic edge-cloud LLM serving, partitioning, offloading, pipeline orchestration, mobility, state migration, and realistic WAN-aware inference** are included.

## P0 — Core / Must Read

### DynoPipe Lineage
- **[ISCA 2026] DynoPipe: Heterogeneous Edge-Cloud LLM Serving with Dynamically Orchestrated Pipeline Boundaries**  
  DOI: https://doi.org/10.1109/ISCA66397.2026.00077
- **[EuroSys 2026] FlexPipe: Adapting Dynamic LLM Serving Through Inflight Pipeline Refactoring in Fragmented Serverless Clusters**  
  Paper: https://arxiv.org/abs/2510.11938
- **[SIGCOMM 2026] Connex: Endpoint Mobility Primitives for Dynamic LLM Serving**  
  Author page: https://yanyinglin.github.io/publications/

### Direct Dynamic Partitioning Competitors
- **[WcCST 2026] DynaSplit: Latency-Aware Dynamic Model Partitioning for Large Language Model Inference in the Edge-Cloud Continuum**  
  DOI: https://doi.org/10.1109/WCCST67302.2026.11496291
- **[FITEE 2025] Adaptive Layer Splitting for Wireless Large Language Model Inference in Edge Computing: A Model-Based Reinforcement Learning Approach**  
  DOI: https://doi.org/10.1631/FITEE.2400468
- **[arXiv 2025] Splitwise: Collaborative Edge-Cloud Inference for LLMs via Lyapunov-Assisted DRL**  
  Paper: https://arxiv.org/abs/2512.23310
- **[arXiv 2025] Memory- and Latency-Constrained Inference of Large Language Models via Adaptive Split Computing**  
  Paper: https://arxiv.org/abs/2511.04002

## P1 — Edge-Cloud LLM Serving / Orchestration

- **[ICC 2025] Distributed Inference Optimization for Large Language Model in Edge-Cloud Collaborative Networks**  
  DOI: https://doi.org/10.1109/ICC52391.2025.11160773
- **[Electronics 2025] DAPO: Mobility-Aware Joint Optimization of Model Partitioning and Task Offloading for Edge LLM Inference**  
  DOI: https://doi.org/10.3390/electronics14193929
- **[ACL 2026] EdgeFormer: Latency-Aware Collaborative Multi-Head Attention of Transformer Inference in Edge Networks**  
  Paper: https://aclanthology.org/2026.acl-long.2007/
- **[ICDCS 2026] TurboInfer: Targeting Age of Model Inference Optimization for Joint Model Inference in Edge Cloud Systems**  
  DOI: https://doi.org/10.1109/2575-8411.2026.00030
- **[arXiv 2026] Efficient and Privacy Aware Edge Cloud Collaborative Inference for Large Language Models**  
  Paper: https://arxiv.org/abs/2607.13093

## P1 — State / KV Migration

- **[ICDCS 2026] Efficient KV Cache Migration for Geo-Distributed LLM Inference in Collaborative Edge Computing**  
  DOI: https://doi.org/10.1109/2575-8411.2026.00033

This paper is especially relevant to DynoPipe because dynamic boundary or endpoint movement is only practical if inference state can migrate cheaply.

## P2 — Background for Split Inference / Edge-Cloud Partitioning

- **[Survey 2025] A Survey on Deep Learning in Edge-Cloud Collaboration: Model Partitioning, Privacy Preservation, and Prospects**
- **[MobiCom 2024] FlexNN: Efficient and Adaptive DNN Inference on Memory-Constrained Edge Devices**  
  DOI: https://doi.org/10.1145/3636534.3649391
- **[JOCN 2025] Joint Optimization of DNN Model Partitioning and Slice Delivery for Distributed Edge-Cloud Inference over Optical Networks**
- **[JPDC 2026] Multi-Modal Model Partition Strategy for End-Edge Collaborative Inference**

These are background only; they are not the main LLM research target.

## Reading Priority

1. DynoPipe
2. FlexPipe
3. Connex
4. DynaSplit
5. Adaptive Layer Splitting for Wireless LLM Inference
6. Efficient KV Cache Migration for Geo-Distributed LLM Inference
7. Distributed Inference Optimization for LLM in Edge-Cloud Collaborative Networks
8. Splitwise
9. Adaptive Split Computing
10. DAPO
11. EdgeFormer
12. TurboInfer

## Excluded on Purpose

Do **not** add papers merely because they contain the word `edge`.

Excluded unless directly tied to partition/orchestration:
- generic speculative decoding / Cassandra
- MoE expert substitution / SMoE
- generic quantization and pruning
- pure on-device inference
- generic cloud LLM serving
- compiler / kernel work with no direct edge-cloud placement implication
