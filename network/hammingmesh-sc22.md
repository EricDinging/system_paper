# HammingMesh: A Network Topology for Large-Scale Deep Learning

## Summary

A flexible network topology that help embed toridal ML communication pattern. HammingMesh combines sparsely connected boards in a dimension-wise (not globally) fully-connected topology.

## Pros
- Decent alltoall and collective bandwidth at reasonable cost

## Cons
- FatTree for reach
- Reducing cost of global scale-out network is at-odds with reducing compute fragmentation

## Question
1. Dragonfly
3. Multiple interfaces per chip
4. Hamiltonian cycles
5. Why Torus behave not as good as ring when the message size is large