# [Optimizing Dynamic Neural Networks with Brainstorm](https://www.usenix.org/conference/osdi23/presentation/cui)

## Problem
- Dynamic NN can adapt sub-networks to inputs during inference
- Existing DL framework and compilers mainly focus on optimizing static NN with deterministic execution
## Challenges
- Traceability of how data are dynamically dispatched to different paths at inference
- Hard for existing tensor-centric frameworks to trace due to misaligned expression granularity

## Observations

## Ideas
- Introduce Cell, key data abstraction that developers express the data granularity where dynamism exists
- Router, interface that let model developers express how cells should be dynamically dispatched
## Results
- Extensive evaluations show Brainstorm brings up to 11.7× speedup (3.29× on average) or leads to 42% less memory consumption for popular dynamic neural networks with the proposed dynamic optimizations
## Application

## Limitation

## Questions