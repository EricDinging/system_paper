# SimAI: Unifying Architecture Design and Performance Tuning for Large-Scale Large Language Model Training with Scalability and Precision

## Summary
SimAI is a LLM performance simulator for large-scale datacenters. It generates accurate estimation of the execution time. 

## Pros
- It is a unified simulator for computation and communication
- Uses a database to cache operator latency in certain GPU architectures
- Enables network architecture and model configuration search


## Cons
- The simulator requires modification whenever the ML frameworks update.
- Introduce dependencies between collectives call
- Need to do multiple measurements for collectives with different input size