# ATLAHS: An Application-centric Network Simulator Toolchain for AI, HPC, and Distributed Storage

## Summary
- Use real trace for benchmarking
- leverages Group Operation Assembly Language (GOAL), allowing users to implement their own trace parsers
- multi-job and multi-tenancy scenarios
## Pros
- Generalize to HPC and cloud workloads
## Cons
- Infers the amount of computation by the collectives
- Does not show how dependency between kernels are constructed
- Modeling intra-node send/recv with computation node, not reflecting the intra-node interconnect contention or latency
- Very simple computation time estimation