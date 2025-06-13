# [RDMA over Ethernet for Distributed AI Training at Meta Scale](https://dl.acm.org/doi/pdf/10.1145/3651890.3672233)
## Problem
- Distributed training imposes the most significant strain on data center networking infrastructure
## Backgrounds
- Inter-GPU communication
    - Inter-node: NVLink
    - Intra-node: 
        - CPU: TCP/IP or modified socket implementation, susceptible to performance degradation
        - Proprietary interconnects: infiniband, NVSwitch, Elastic Fabric Adpator
        - RDMA: RoCE
## Challenges


## Observations

## Ideas

## Contribution

## Methods
- Dedicated backend network for LLM training
- New routing scheme: ECMP (equal cost multi-path) has poor performance; adopt a combination of centralized traffic engineering and an enhanced ECMP scheme
- Congestion control for collectives: challenging to tune DCQCN; designed a receiver-driven traffic admission via the collective library 
## Results

## Application

## Limitation

## Related concepts

## Questions