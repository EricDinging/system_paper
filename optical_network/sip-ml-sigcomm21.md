# SiP-ML: High-Bandwidth Optical Network Interconnects for Machine Learning Training

## Summary
- Optimize parallelization algorithm for optical network to satisfy the network degree constraint
- Propose two optical network: (1) OCS and (2) Ring
- Sip-ML cluster consists of disaggregated GPUs, each equipped with Tbps SiP interfaces

## Observation
- The partitioning is fine-grained within model parallelism group, leading to GPU workload imbalance
- The MP and DP group communication fall under the same degree constraints (no reconfiguration in-between)

## Cons
- No convergence proof of the model placement algorithm
- Sip-Ring reconfigures based on traffic pattern read from the buffer counters through PCIe, introducing delay

## Questions
- What kind of topology does Sip-Ring provide?
