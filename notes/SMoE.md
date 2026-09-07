# SMoE

## Metadata
- Title: SMoE: An Algorithm-System Co-Design for Pushing MoE to the Edge via Expert Substitution
- Venue / Year: ISCA 2026
- Paper: https://arxiv.org/abs/2508.18983
- Tags: `edge` `moe` `expert-substitution` `memory` `hardware-aware`

## 1. Problem
Mixture-of-Experts models are attractive because only a subset of experts activate per token, but the complete expert set creates a major memory and placement challenge on edge devices.

## 2. Key Idea
Use expert substitution and algorithm-system co-design to reduce the need to keep every expert resident on the edge while preserving useful model capacity.

## 3. Why It Matters Here
SMoE represents the model/system co-design branch of edge LLM inference. It is useful as a contrast with DynoPipe: rather than moving arbitrary transformer layers between edge and cloud, it changes how the model itself is executed under edge constraints.

## 4. Questions to Extract
- How are substituted experts selected?
- What accuracy/perplexity cost is introduced?
- How much memory is saved?
- Does expert substitution reduce communication compared with expert offloading?
- What happens under dynamic expert popularity?
- Can expert placement be coordinated with edge-cloud scheduling?

## 5. Relation to DynoPipe
DynoPipe changes **placement of model stages**; SMoE changes **the model execution structure** to fit the edge. Future systems may need both model adaptation and runtime orchestration.

## 6. Reproduction Status
- [ ] code found
- [ ] expert-selection mechanism understood
- [ ] baseline runnable
- [ ] key result reproduced
