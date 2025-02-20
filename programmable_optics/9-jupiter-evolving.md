# Jupiter Evolving: Transforming Google’s Datacenter Network via Optical Circuit Switches and Software-Defined Networking

## Summary
This paper introduced a network fabric based on OCS that is incrementally deployable.  The researchers use the combination of traffic and topology engineering to achieve similar throughput as Clos fabrics using direct-connect fabrics. The minimum latency of flows is dropped by 7-11% and 24% for 99% tail latency.

## Pros
- The paper introduces a very interesting motivation: updating spine layer for optimal performance for all blocks is resource-intensive, so it might as well be removed entirely.
- Hierarchical OCS for failure domain minimization.

## Cons
- The decision-making behind topology and traffic engineering is not clear. It seems that most of the time the cluster will use traffic engineering.
- The central controller may not scale well.
