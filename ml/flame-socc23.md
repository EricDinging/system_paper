# [Flame: Simplifying Topology Extension in Federated Learning](https://arxiv.org/pdf/2305.05118)
## Problem
1. Improve flexibility of FL deployments, support various topologies (hierarchical and hybrid) as well as algorithms

## Backgrounds
- Creating and deploying models in geo-distributed settings requires support from resource orchestrators, model registry and monitoring tool integration
- AI automation platform lacks support for programmatically extending the topology of the deployed jobs
- FedML, FedScale, Flower, and PySyft API and client-server based abstraction lacks extensibility (extending to different topologies)
## Challenges

## Observations
1. FL system needs to be flexible and easily extensible (FedScale lacks)
2. Decouple the management of learning logic, compute and data
## Ideas
1. Flame introduces a new abstraction called Topology Abstraction Graph (TAG)
2. Provide interface to describe and integrate with different compute infracstructure and dataset providers
## Contribution

## Methods

## Results

## Application

## Limitation

## Related concepts
1. MQTT vs. gRPC
2. Communication collectives like ring-all-reduce
## Questions