# [Karma: Resource Allocation for Dynamic Demands](https://www.usenix.org/system/files/osdi23-vuppalapati.pdf)
## Problem
- Designing resource allocation mechanism that achieve Pareto efficiency and strategy proofness
    - Fairness
        - Max-min
        - Strict partitioning
- Fair resource allocation in a system where user demands are dynamic
    - How to ensure long term fairness
## Challenges

## Observations
- Classical max-min fairness algorithm for resource allocation have strong properties only under the strong assumption of user demands being static over time
- Max-min fairness guarantees fail for dynamic user demands
- Periodically run max-min fairness does not ensure fairness over aggregated received resources
## Ideas
- Credit-based resouce allocation algorithm
- In each quantum, users donate their unused resources and are assigned credits when other users borrow these resources
- Karma performs prioritized resource allocation based on users' credits

## Results
- Theoretically establish Karma guarantees related to Pareto efficiency, strategyproofness, and fairness for dynamic user demands
- Karma guarantees Pareto efficiency at all times, in each quantum
## Application
- Is able to reduce disparity in performance across users to a bare minimum while maintaining Pareto-optimal system-wide performance

## Limitation

## Questions