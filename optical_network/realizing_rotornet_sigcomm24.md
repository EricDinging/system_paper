# Realizing RotorNet: Toward Practical Microsecond-scale Optical Networking

## Summary
Authors provide the first real-world measurements of Linux TCP
throughput and host-to-host latency in an operational RotorNet,
achieving 98% of link rate with 99th-percentile ping times faster
than commodity packet-switching hardware.

They develop and deploy a novel end-host-based masking technique, allowing TCP transfers to extract 99.5% of the link capacity

## Background
1. No commercial deployments of fast optical circuit switching (under microseconds)

## Design
1. RotorNet employs a fixed, cyclic connectivity schedule at the physical OCS level and a version of Valiant
load balancing called RotorLB to route traffic over the prede-
termined (but time-varying) optical paths. This provides 50-100%
of ideal throughput regardless of traffic skew while avoiding the
complexity of a centralized scheduler.
2. Indexing routing table based on IP and topoligy (time)
3. Two options for forwarding traffic through the network: (1) a low-latency, but less bandwidth-efficient service based on
Opera’s multi-hop “cut-through” routing and (2) a higher-latency, but more bandwidth-efficient service based on one- or two-hop
“store and forward” routing as in RotorLB.
4. NIC performs forwarding.

## Pros

## Cons
1. Each node in the optical network requires multiple distinct uplinks,
one per rotor switch.