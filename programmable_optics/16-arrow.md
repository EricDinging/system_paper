# ARROW: Restoration-Aware Traffic Engineering

## Summary
The paper argues that optical link cut is not a binary event. An optical link cut is partially restorable and the routers and switches could be re-utilized. ARROW is a traffic engineering system that determines the mapping between IP flows to partially available optical links that increases the availability and the utilization of the network. Arrow uses a two-stage approach to first find the possible restoration candidates and then appropiate tunnel allocations. It's shown in simulation that Arrow supports 2x-2.4x more demand with high availability.

## Pros
1. Propose scalable lottery ticket abstraction to solve optimization problem.
## Cons
1. ROADAM could change wavelength of a network flow, potentially solving wavelength continuity constraint. The paper does not address this issue.
