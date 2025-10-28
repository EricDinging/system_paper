# FreeFlow: Software-based Virtual RDMA Networking for Containerized Clouds

## Summary
RDMA and containerization are in conflict with each other.
- Isolation
- Portability
- Controllability

It is difficult to modify the control plane states (e.g., routes) in hardware in shared cloud environments, while it is also hard to control the data path since traffic directly goes between RAM and NIC via PCIe bus. And there is no mature RDMA virtualization solutions for containers.

FreeFlow is a software virtual switch running on each server to virtualize RDMA on commodity RDMA NICs.

## Challenges
1. RDMA requires a NIC to manipulate memory buffers and file descriptors, while applications inside containers do not directly interact with the NIC due to network virtualization.
    - FreeFlow and a container share the same memory (§4.3) and file descriptor, any operations on the underlying physical RDMA NIC will automatically take effect inside the container.
    - convert resource from non-shareable to shareable in application
2. Throughput and latency that is comparable to bare-metal RDMA
    - zero-copy design for throughput
    - a shared memory inter-process channel with CPU spinning for latency


## Design
FreeFlow intercepts the communication between applications and physical NICs, and performs control plane and data plane policies inside the software FreeFlow router which runs as another container on the host machine.

- FreeFlow network library
- FreeFlow software router
    - implements the data-plane resource policies, e.g., QoS, by controlling the shared-memory channel between containers and FFR

- FreeFlow orchestrator

## Implementation
- The primary challenge is to support one-sided operations and event-based completion notifications.
    - FFR needs to busy pulling
    - Solution is to transparently share memory and file descriptors between application and FFR
- One sided operation, mem pointer is not known to FFR in remote
    - Relies on key value store in FFO for mapping between mem and smem in remote note
- One sided operation requires FFR receiver to keep pulling smem
    - Allocating shared buffers using new APIs for application