# Cassandra

## Metadata
- Title: Cassandra: Enabling Reasoning LLMs at Edge via Self-Speculative Decoding
- Venue / Year: ISCA 2026
- Paper: https://arxiv.org/abs/2605.26558
- Tags: `edge` `self-speculative-decoding` `reasoning-llm` `hardware-aware`

## 1. Problem
Reasoning LLMs are expensive to decode on resource-constrained edge hardware. Adding a separate draft model may itself consume too much memory and compute.

## 2. Key Idea
Use self-speculative decoding so that the target model, or a cheaper execution path derived from it, supplies draft tokens and reduces the cost of autoregressive generation without requiring a fully separate draft model.

## 3. Why It Matters for This Repository
Cassandra represents an alternative to pure Edge→Cloud model partitioning. Instead of splitting one model across a WAN boundary for every generation step, it attacks Decode cost algorithmically on the edge side.

## 4. Questions to Extract from the Paper
- What exact draft mechanism is used?
- What layers/blocks are skipped or reused?
- How is acceptance rate controlled?
- What hardware is used for the edge evaluation?
- What happens for long reasoning traces?
- What are the memory and latency trade-offs?
- Can its self-speculative path be combined with cloud verification or phase-aware placement?

## 5. Relation to DynoPipe
DynoPipe focuses on **where computation runs**; Cassandra focuses on **how Decode computation is reduced**. Their combination may be useful if a future system separates Prefill placement from Decode acceleration.

## 6. Reproduction Status
- [ ] code found
- [ ] model setup understood
- [ ] baseline runnable
- [ ] key result reproduced
