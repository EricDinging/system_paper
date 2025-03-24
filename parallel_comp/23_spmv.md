# Implementing Sparse Matrix-Vector Multiplication on Throughput-Oriented Processors

## Please write a summary of the paper [from 3 to 6 sentences].

The paper first emphasizes the importance of efficient memory access patterns for sparse matrix workloads. And it highlights various forms of irregularity for sparse matrix operations is one of the biggest bottleneck. It proposes approaches that aim to minimize execution and memory divergence caused by the potential irregularity. Achieving 2.8x speed up on previous implementation.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
- The work considers different kind of input matrices, from highly regular diagonal matrices to completely unstructured matrices with highly varying row lengths.
- The work emphasizes a very interesting observation: as the parallel granularity is refined, the impact of thread workload imbalances becomes a significant concern.
- The work considers different input precision and performs rather complete ablation study.

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
- The implementation is highly coupled to specific hardware version available at that time.
- The paper does not clearly specify whether the implementation is memory-bound or compute bound.
- The work does not consider transformations such as row permutation that globally restructure the matrix.


## Please provide a question for in-class discussion.
- Is texture cache also exist on modern GPUs? The proposed algorithm use this hardware feature. Does it mean the method should be changed for modern hardware?

## Please provide a question for in-class discussion.
- What would be the cost of transforming matrix before computation? If the cost is small enough or is optimizable, would it be wise to do the dynamic matrix transformation?

