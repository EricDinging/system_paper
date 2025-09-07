# OPTIREDUCE: Resilient and Tail-Optimal AllReduce for Distributed Deep Learning in the Cloud

## Summary
- Introduce transpose allreduce to reduce the impact of lost gradient by establishing direct p2p communication
    - Smaller number of rounds
    - Smaller impact when one communiction is lost
- Introduce unreliable bounded transport (adaptive timeout, adjust the number of concurrent sender per receiver)
- Hadamard transform for unbiased estimate of the gradients for minimal loss under any drop pattern
## Pros

## Cons
- Only implemented in GLOO (CPU-based)