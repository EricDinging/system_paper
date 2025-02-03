# Title

## Summary
The paper introduces C-Through, a hybrid data center network consisting of electrical and optical networking planes. The electrical networking plane is used for small, latency-sensitive flows, while the optical networking plane is used for big, bandwidth-sensitive flows. C-Through relies on end-hosts for traffic monitoring and de-multiplexing instead of applications and switches, making it easy to implement.

## Pros
1. C-Through implements traffic measurement and control in end-host kernel without the need of application changes, leading to its ease of implementation.
2. C-Through can scale theoretically to 1000 racks in datacenters.

## Cons
1. This work has not been implemented over real OCS switch.
2. This work has not discussed the maximum duration one flow could wait for a link to be established.
3. There is no evaluation/simulation on scalability.

## Future work
1. Develop switch-based traffic monitoring and de-multiplexing
2. Develop protocols that could operate on top of fast-changing topologies with a circuit visit delay.
3. Implement broadcast/multi-cast using optical network.
4. Explore application and circuit switching (topology) co-design.


