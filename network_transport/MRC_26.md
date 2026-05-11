# Resilient AI Supercomputer Networking using MRC and SRv6

## Summary

1. MRC, new RDMA-based transport, eliminating the issue of flow collision
    - Packet spraying
    - Adaptive load balancing based on ECN
    - Out-of-order memory placement of received data
    - Selective retransmission
    - Pakcet trimming to mitigate incast
2. Multi-plane Clos topologies, reaching 100K GPU, two-tier network with physical redundancy.
3. Static source-routing to allow MRC the freedom to bypass failures by itself.

## Implementation
1. MRC leverages and extends the existing Verbs API but AI workloads only require a subset
    - RDMA write and write-with-immediate
    - Static source-routing?
2. Multi-plane topology
    - Reliability, cost and power reduced, lower hops
    - Challenges
        - the workload needs to be able to survive link and NIC port failures
        - Load balance across all the many paths within a plane without performance loss due to flow collision
            - Hard to do with single-path transport protocol
3. Disable PFC
    - best-effort Ethernet and out-of-order delivery
4. Fast selective retransmission, using selective ACK
5. Use packet trimming, and packet is priority-forwarded to the destination
6. Static segment routing
    - when running MRC, dynamic routing caused more problems than it solved
