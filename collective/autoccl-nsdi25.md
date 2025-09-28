# AutoCCL: Automated Collective Communication Tuning
for Accelerating Distributed and Parallel DNN Training

## Summary

- Dynamically tune NCCL implementation parameters and resource allocation parameters
- Build a performance model and subspace-based tuning method.
    - Divide the subspace based on \<algorithm, protocol, transport\>. Then determine the optimal combination of <Number of channels, number of threads, chunk size>

## Motivation
- Insight: Current cost model assume bw and latency are fixed between GPUs. But the bw is affected by message size, cluster topology, congestion, and concurrency.

## Design
- $\beta(NC, NT, C) = min(\beta_0(NC, C), \beta_1(NC, NT))$. $\beta_0$ is the transport bandwidth, and $\beta_1$ is the protocol (computation) bandwidth

## Implementation
- Use a leader-worker model for configuration broadcast.

## Cons
- Does not discuss whether the model fits real-world

## Question
1. Is the tuning depends on communication tasks? 
