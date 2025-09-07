Concerto: Automatic Communication Optimization and Scheduling for Large-Scale Deep Learning
## Summary
Abstracts the communication optimization as a resource-constrained project scheduling problem.
1. PyTorch function trace: fx Graph
2. traced fx graph -> ConcertIR, hybrid graph containing computation and communication operators
3. Auto-decomposition, identifies critical communication and decompose their context
4. Scheduling, generating the topological order of the graph for runtime execution, applying optimizations such as communication fusion.


## Pros
1. With out the need to run the workload in parallel at first 
2. Optimizes any parllelism approach
3. Insight:
- Async comm operators, maximizing parallel processing through operator order scheduling
- sync comm operators, decomposing contextual conputation creates optimization opportunities for overlap
## Cons
1. The work do not focus on the communication overhead from pipeline model parallelism
2. Assume it’s common for one computation and one communication to be performed simultaneously in most cases.
3. Does not specify "commodity communication (non-NVLink)"

## Question
1. PyTorch bucket size
2. Aten operators
3. Pytorch compilation process
4. Torch._custom_ops
5. PyTorch communication time is lower than JAX
6. XLA's heurisic algorithm cannot adapt to different hardware environments.
