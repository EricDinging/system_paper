# [Karma: Resource Allocation for Dynamic Demands](https://www.usenix.org/system/files/osdi23-vuppalapati.pdf)
## Problem
- Fair resource allocation in a system where user demands are dynamic
## Challenges

## Observations
- Classical max-min fairness algorithm for resource allocation have strong properties only under the strong assumption of user demands being static over time
## Ideas
- Credit-based resouce allocation algorithm
- In each quantum, users donate their unused resources and are assigned credits when other users borrow these resources
- Karma performs prioritized resource allocation based on users' credits

## Results
- Theoretically establish Karma guarantees related to Pareto efficiency, strategyproofness, and fairness for dynamic user demands

## Application
- Is able to reduce disparity in performance across users to a bare minimum while maintaining Pareto-optimal system-wide performance

## Limitation

## Questions