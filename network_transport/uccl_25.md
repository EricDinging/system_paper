# An Extensible Software Transport Layer for GPU Networking

## Summary
- Goal: flexibility, extensibility, higher performance without expensive hardware changes or hacky modifications on existing RDMA stack
- Efficient control plane and data plane separation for ML communication transport
    - leverages RDMA Unreliable Connection (UC) to bypass hardware-baked CC and packet reliability logic, and uses RDMA immediate data to pass transport control states between sender and receiver GPUs.
- Achieve hardware-level performance with control plane based on CPU
    - Uses GPUDirect to remove CPU overhead
    - employs control coalescing
- Congestion control
    - Receiver-driven EQDS for in-cast traffic pattern in MoE
- Multi-pathing
    - Uses 256 QPs
    - Amortized QP context swapping overhead due to MTU-sized packets
- Reliability
    - Selective retransmission
    - Existing PFC methods could cause deadlocks, HOL blocking, and victim flows

## Pros

## Cons
