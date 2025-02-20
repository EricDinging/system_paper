# GE-SpMM: General-Purpose Sparse Matrix-Matrix Multiplication on GPUs for Graph Neural Networks

## Please write a summary of the paper [from 3 to 6 sentences].
This paper presents a SpMM-based design based on CSR for GNN applications using GPU. GE-SpMM introduces two techniques: Coalesced Row Caching and Coarse-grained Warp Merging, improving the efficiency of global data access. This techniques contribute to 1.25× and 1.51× speedup.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
- The use of the CSR format ensures compatibility with existing GNN frameworks.
- The paper considers different matrix sizes and provides adaptive solutions.
- CRC and CWM shows a deep understanding of GPU architecture and memory access patterns.

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
- There is no scalability evaluation for larger graph sizes.
- The discussion on how GE-SpMM performs on different types of graph is limited.
- I would love to see the performance gain on more GPUs of different models.

## Please provide a question for in-class discussion.
Will the performance over baseline be as significant as shown in this paper when applying this techniques to other GPU models?

## Please provide a question for in-class discussion.
All these frameworks are built based on Nvidia stack. Are they easy to be migrated to AMD's ROCm software stack?



