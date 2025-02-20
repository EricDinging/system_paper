# TPU v4: An Optically Reconfigurable Supercomputer for Machine Learning with Hardware Support for Embeddings

## Summary
This paper introduced TPUv4 supercomputer architecture. The supercomputer uses proprietary chips, interconnected by direct-connect fabrics within a block and across blocks. The intra-block interconnect uses electrical mesh network, and the inter-block interconnect uses OCSes to implement direct-connected topology.

## Pros
- The researchers address the fault tolerance measures using indirect routing.
- The research demonstrates a successful large-scale deployment of OCSes.

## Cons
- The exact routing strategy is not clearly defined.
- The scale is bottlenecked by the number of ports on the OCS.
