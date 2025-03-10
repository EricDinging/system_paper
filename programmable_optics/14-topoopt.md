# TOPOOPT: Co-optimizing Network Topology and Parallelization Strategy for Distributed Training Jobs

## Summary
Topoopt is a direct-connect fabrics for DL workloads using optics. Based on the communication patterns of AllReduce and its mutability characterestics, TopoOpt is able to construct efficient network topologies. The researchers demonstrate the performance of TopoOpt on a 12-node direct-connect prototype with RDMA enabled, and also through large-scale simulation, enabling significant performance enhancement 

## Pros
- The work leverages cross-stack optimization based on insights from traffic pattern analysis.

## Cons
- The topology needs to rely on traffic aggregation (TOR) to scale.