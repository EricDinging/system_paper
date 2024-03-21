# [LIFL: A Lightweight, Event-driven, Serverless Platform For Federated Learning ](link)
## Problem
- FL aggregation, hierarchical aggregation
## Backgrounds
- Current FL stack, always on style leads to resource wastage as FL workload is typically dynamic
- Loose coupling of data plane components is a barrier to achieve efficient aggregation
- Current serverless frameworks use constantly-running components, not event-driven
    - they mainly support serverless functions, which are ephemeral and stateless, only supporting indirect networking 
    between functions
- Current autoscaling is agnostic of the hierarchical structure of FL aggregation.
## Challenges


## Observations

## Ideas
- Serverless
- Hierarchical aggregation
- Intra-node shared memory processing
- Locality-aware placement policy
- e-BPF event-driven processing
- Reuse runtimes
- In-place message queueing
## Contribution

## Methods

## Results

## Application

## Limitation
1. No CDN, all servers are in one nodes
2. How eager aggregation works with hierarchy?
## Questions