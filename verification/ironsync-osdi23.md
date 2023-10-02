# [Sharding the State Machine: Automated Modular Reasoning for Complex Concurrent Systems](https://www.usenix.org/system/files/osdi23-hance.pdf)
## Problem
- Hard to debug concurrent code
- Aggressively optimized systems that use custom sync tools, entangling synchronization logic with application logic
- Formal verification struggle to reach production-scale shared memory systems
## Challenges

## Observations

## Ideas
- Partition system-level proof 
- IronSync developer use an ownership type system. Owned value must be held or referenced by exactly one variable
- Developer reason about the logical correctness 
- Localized transition system abstracts the state each threads act upon. Ironsycn abstracts LTS into a simplified program
- The developer writes their implementation and performs all of the reasoning above in an extended version of the Dafny
language augmented with the trusted axioms and memory primitives in IronSync’s framework

## Results

## Application

## Limitation
- IronSync does not verify liveness, termination, or deadlock-freedom.

## Questions