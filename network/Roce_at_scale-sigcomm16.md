# RDMA over Commodity Ethernet at Scale

## Motivation
- CPU spends ~10% of time performing checksum offloading, large segment oﬄoad (LSO), receive side scaling (RSS) and interrupt moderation for TCP.
- TCP incurs latency: kernel processing, packet drops
- Need for congestion control for RDMA: DCQCN

## RDMA
- RDMA needs a lossless network
- PFC prevents packet loss, but has HOL blocking problem, potential for deadlock.
- UDP header is useful for ECMP-based multipathing
- Congestion control to reduce reliancy on PFC
- Coexist with TCP
- RDMA livelock
    - go-back-to-0 retransmission logic
- Deadlock even with no circular dependency
    - unexpected interaction between PFC and Ethernet packet flooding broke the up-down routing

## Solution
- DSCP-based PFC
    - VLAN based PFC requires specific port mode, causing packet drop during OS update
    - No good way to preserve VLAN metadata when using IP forwarding
    - DSCP field in IP header carries packet priority information
- Go-back-N to remove livelock
- Drop packet when ARP entry is incomplete

## Deployment
- The PFC configuration has a global part which reserves buﬀer size, classifies packets into diﬀerent traﬃc classes based on the DSCP value, maps diﬀerent traﬃc classes into diﬀerent queues, and assigns diﬀerent bandwidth reservations for diﬀerent queues.