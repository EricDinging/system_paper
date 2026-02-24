# MSCCL++: Rethinking GPU Communication Abstractions for AI Inference

## Summary
a design methodology for developing high-performance, portable communication kernels.
1. Primitive API exposes minimal hardware abstractions while hiding the complexities of synchronization and consistency
2. a higher-level DSL for application developers to implement workload-specific communication algorithms
3.  a library of efficient algorithms implementing the
standard collective API
## Pros
- Allow fine-grained oeverlapping of compute and communication
- Have abstractions over port, memory, and switch channel
- DSL provides a global thread-block view
## Cons

