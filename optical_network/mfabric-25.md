# mFabric: An Efficient and Scalable Fabric for Mixture-of-Experts Training
## Summary
Use regional OCS block to implement MoE All2All traffic. Design networking stack to predict and reconfigure topology. Achieve the pareto frontier of cost and performance for MoE models.

## Pros
1. The design is very simple. Change some of the NIC setups from packet switch connection to OCS connection.
2. Comparable performance to fat tree and rail-optimized topology
3. Working prototype with commodity OCS

## Cons
1. Require network partioning into several OCS-connected regions
2. Split the eight NICs to EPS domain and OCS domain, introducing potencial contention in the NVLink domain
3. Does not mention that EP is typically co-implemented with DP and how DP traffic is handled.
4. multiple steps involving inter and intra-host communication for all2all due to limited NIC for EP
5. OCS can not handle all of the EP traffic

## Observation
1. Their observations indicate that the overall turnaround time of one reconfiguration is predominantly influenced by the physical link initialization and NIC device initialization.