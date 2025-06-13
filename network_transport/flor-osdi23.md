# [Flor: An Open High Performance RDMA Framework Over Heterogeneous RNICs](https://www.usenix.org/system/files/osdi23-li-qiang.pdf)
## Problem
- Datacenter applications have been increasingly applying RDMA for ultra-low latency and low CPU overhead
- RDMA-capable NIC of different vendors or generations do not cooperate well
- Bandwidth imbalance in the production network
- Introduce new root causes of the PFC (priority flow control) storms
## Challenges

## Observations
- RNIC heterogeneity
## Ideas
- Provide a unified hardware data plane atop heterogeneous RNICs and a flexible software control plane
- The software plane performs congestion control and reliability management in large-scale lossy Ethernet with no PFC dependency

## Results
- Flor achieves comparable performance to vanilla RDMA in both testbed and production clusters
- Mitigates the performance gap of CX-4 and CX-5 RNICs from 24.3% to 1.3%

## Application

## Questions