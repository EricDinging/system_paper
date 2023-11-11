# [Sol: Fast Distributed Computation Over Slow Networks](https://symbioticlab.org/publications/files/sol:nsdi20/sol-nsdi20.pdf)
## Problem
1. Modern execution engine has targeted network with low latency and high bandwidth, late binding before execution works well when the network is well-provisioned
2. Under-provisioned network can lead to large CPU underutilization 
3. Coupling the provisioning of communication and computation lead to HOL
## Challenges

## Observations
Design space
1. Coordination time
2. Communication time
3. Computation time
4. Queueing time
## Ideas
1. Early binding control plane decisions over the WAN, late bind workers in LAN for flexibility
2. Decouple computation from communication, scale down CPU requirement to match available bandwidth
## Methods

## Results

## Application

## Limitation

## Questions