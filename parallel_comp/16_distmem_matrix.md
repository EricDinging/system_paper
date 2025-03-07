# Distributed-Memory Parallel Algorithms for Sparse Times Tall-Skinny-Dense Matrix Multiplication

## Please write a summary of the paper [from 3 to 6 sentences].
This paper evaluates the performance of various techniques for performing SpMM using distributed GPU clusters. The paper shows that the choice of distributed algorithm (A-Stationary, B-Stationary, 1.5D algorithms, 2D algorithms) and implementation depend on the cost of communication for specific matrix dimension and local SpMM operation.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
- This work provides a systematic analysis on the choice of algorithms and implementations for distributed SpMM workloads.
- This work considers various matrix sparsity levels and dimensions.
- It provides an overview of the optimization space, from application, data moveement point of view to the network communication point of view.

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
- This work primarily focuses on static partitioning strategies and does not explore load-balancing techniques.
- The work does not consider using asynchronous operatives in CUDA in addition to RDMA operations.
- The work assumes the network is congestion-free.

## Please provide a question for in-class discussion.
Could the result be used for constructing a performance simulator for SpMMM workloads to inform users the optimal implementation configurations?

## Please provide a question for in-class discussion.
Can the algorithm proposed in this work be adapted to irregular sparse matrices?
