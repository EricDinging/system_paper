# [Skyplane: Optimizing Transfer Cost and Throughput Using Cloud-Aware Overlays](https://www.usenix.org/system/files/nsdi23-jain.pdf)
## Problem
- Slow transfer lock in data
- High egress fees
- Solve data gravity problem
## Challenges

## Backgrounds

## Observations
- Reasons why slow
    - Congestion along direct path
    - Poor peering between providers
    - Packet loss from physical layer
    - Throttling from cloud providers
## Ideas
- Profiling
- Planning: centralized LP planner finds optimal transfer path
    - Overlay routing to circumvent slow links
    - Throughput is relatively stable, so centralized planning is feasible
- Execution: provision ephemeral gateway VMs from plan
    - Elastic
    - Parallel VMs per region to avoid provider throttling
    - Parallel TCP connections
    - Cut cost: compression, network tiers
## Contribution

## Methods

## Results
- 1.3x speedup with 30% less cost compared to Ron
## Application

## Limitation

## Questions