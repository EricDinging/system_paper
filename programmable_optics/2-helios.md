# Helios: A Hybrid Electrical/Optical Switch Architecture for Modular Data Centers

## Summary
Helios is a hybrid datacenter network design that integrates both optical and electrical switching components. This architecture aims to leverage the strengths of both technologies to create a more efficient and flexible network infrastructure for modular data centers.


## Pros
1. No modifaction is needed by Helios for application and end hosts.
2. The paper quantifies the benefit of cost and power, which are important metrics.
3. The paper demonstrates the need for optical switching by addressing the issue of underutilization in full-bisection bandwidth scenarios
4. The architecture provides a distinct separation of traffic between the electrical and optical planes, allowing for optimized routing and resource allocation.

## Cons
1. Scalability of topology manager is not addressed.
2. The work has not evaluated actual workload

## Future work
1. Explore the integration of Helios with SDN.
2. Research methods to enhance the scalability of the topology manager, possibly through distributed management approaches.
3. Transport layer with switching layer integration.
4. Performance vs. fairness for optical switching.
