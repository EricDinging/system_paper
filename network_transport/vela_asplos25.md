# Vela: A Virtualized LLM Training System With GPU Direct RoCE

## Motivation
Can we build a cloud (virtualization-based) system for LLM training workloads with off-the-shelf hardware and a primarily open-source system stack while delivering HPC-like performance

## Solution
1. Linux-KVM-based virtual machines
2. vendor-agnostic flow-based software-defined networking (SDN)
    - we utilize programmable NICs to offload network virtualization processing to the NIC hardware.
3. leverages Single Root I/O Virtualization (SRIOV) technology to create virtual functions (VFs) on top of network interface cards (NICs)
4. vendor-agnostic hardware-software co-design approach for congestion management
