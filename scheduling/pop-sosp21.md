# [Solving Large-Scale Granular Resource Allocation Problems Efficiently with POP](https://dl.acm.org/doi/pdf/10.1145/3477132.3483588)
## Problem
- Resource allocator hit bottlenecks when the numbers of clients and resources increase
    - Relie on heuristics, which often do not extend to slightly modified objectives
## Backgrounds

## Challenges


## Observations

## Ideas
- Granular resource allocation
    - Scale: hundreds or more clients and resources
    - Small clients
    - Client resource fungibility
- In the case where the client or resource is not granular, use two granularization techniques
    - client splitting
    - resource splitting


## Contribution

## Methods
- Randomly partition systems into sub-systems
- Reuse same problem formulation for each sub-problem
- Concatenate allocations
## Results
- Empirically, show that POP's resource allocations are nearly optimal on several optimization problems

## Application

## Limitation

## Questions