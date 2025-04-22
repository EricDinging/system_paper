# FALCON: Pinpointing and Mitigating Stragglers for Large-Scale Hybrid-Parallel Training

## Summary
Categorize stragglers into computation fail-slow and communication fail-slow. Comp fail-slow is transient and has less impact on end-to-end performance. Comm fail-slow could be more persistent.

Falcon proposes four tiers of strategies:
1. Do nothing
2. Remap DP batch across GPUs
3. Adjust parallelization strategies
4. Migration