# High Performance Unstructured SpMM Computation Using Tensor Cores

## Please write a summary of the paper [from 3 to 6 sentences].
This paper introduces Sparse Matrix Matrix Tensor Core-accelerated library for sparse matrix multiplication application. Tensor cores traditionally place constraints on sparse matrix data structure which however is gaining traction from applications. SMaT uses CUDA MMA API and sparse matrix permutation to improve performance. It outperforms SOTA by 2.6x on average.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
- The performance gained (126x in maximum) is exciting.
- The work proposes a theoretical model for library performance.
- The evaluation provided performance comparisons on individual workloads.

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
- The framework is highly tied to CUDA API, restricting its interoperability.
- The paper does not discuss potential limitations where SMaT might not perform optimally.
- There is limited discussion on the scalability of SMaT.

## Please provide a question for in-class discussion.
- Could the techniques presented in SMaT be extended to SpMV?

## Please provide a question for in-class discussion.
- How does the permutation technique specifically interact with the structure of Tensor Cores to improve performance?



