# [Janus: A Unified Distributed Training Framework for Sparse Mixture-of-Experts Models](https://dl.acm.org/doi/pdf/10.1145/3603269.3604869)
## Problem
- Training Mixture-of-Expert is a promising architecture to scale models
- Expensive to train MoE, due to All-to-All communication between layers

## Challenges

## Observations

## Ideas
- Keep experts in-place -> keep data in-place
- Janus supports asynchronous communication
- Reduce traffic by sharing the fetched experts in the same machine
- Implement a topology-aware priority strategy to utilize intra-node and inter-node link when scheduling "fetching expert"

## Results
- Janus can reduce the traffic up to 16× and achieves up to 2.06× speedup compared with current MoE training system

## Application

## Limitation

## Questions