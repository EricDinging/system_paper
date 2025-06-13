# RDMA over Ethernet for Distributed AI Training at Meta Scale
By segregating Frontend and Backend networks, employing various routing schemes, and optimizing collective traffic patterns, the researchers have been able to build a performant and reliable network infrastructure.

## Routing

Poor performance of ECMP

Deployed a combination of centralized traffic engineering and an Enhanced ECMP scheme to achieve optimal load distribution for training workloads.

ECMP causes unevened flow to link mapping when the workload allocation is fragmented or there is network failures.

TE enables more balanced link utilization. However, it's prone to lower performance when there are network failures.

## Transport

Find it challenging to tune DCQCN

Designed a receiver-driven traffic admission via the collective library to achieve superior performance.

1. Find the number of channels and channel buffer sizes across various triaining job sizes and collective types.

2. Implement high priority queueing at switches for CTS packets.

## Collectives
1. No awareness of network topology
- Network-topology-aware rank assignment
2. Assume very low RTT
3. Assume using an adaptive routing mechanism
4. A non-blocking topology without over-subscription

## Cons

No end-to-end measurement
