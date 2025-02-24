# Asynchronous Distributed-Memory Parallel Algorithms for Influence Maximization

## Please write a summary of the paper [from 3 to 6 sentences].
This paper proposes distributed-memory parallel algorithm for Influence maximization problem. The approach fully distribute the input graph instead of replicating, reducing memory pressure. To cope with the communication demand, the work uses fine-grained asynchronous communication scheme. The design
and implementation can achieve up to 29.6× speedup over the MPI-based state-of-the-art on synthetic and real-world network graphs.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
1. The work solves a large-scale problem from two angles: (1) better parallelization technique and (2) better communication schedule, which I find very inspriing.
2. The work includes a very interesting scaling plot, which shows the scalability of the system.

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
1. The work does not include memory usage vs. worker (vs. problem scale) plot in evaluation.
2. The communication scheme efficiency seems highly depends on the non-blockingness nature of the network. They do not discuss the network requirements.


## Please provide a question for in-class discussion.
The authors claim the implementation of the two main approaches as one of the two contributions. I wonder whether they can use the off-of-the-shelf communication library such as NVSHMEM for their usecases.

## Please provide a question for in-class discussion.
Can the approach be adapted to other graph problems? In my opinion, the techniques used are general.


