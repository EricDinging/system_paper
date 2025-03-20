# MCCS

## Summary
- Cloud provider to assume responsibility for choosing the collective communication strategy on behalf of the tenant

## Design
- Tenant calls high-level collective communication interface
- Cloud provider could do joint-optimization
- 

## Cons
- MCCS need to determine routing when a collective is issued, which may incur latency.

## Question
1. Without topology information, randomly assign ranks to workers in different racks could lead to the ring to cross racks back and forth multiple times, causing substantially more inter-rack traffic than necessary. Is this the case? Does NCCL ensure a ring ordering
2. NCCL leaves the optimization of inter-host topology to users? Therefore, users must carefully design the GPU-to-rank mapping
3. Intra-host optimization presents issues in public cloud settings as well due to virtualization.
4. Transport agent in NCCL