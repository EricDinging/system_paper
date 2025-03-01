# Communication-optimal parallel 2.5D matrix multiplication and LU factorization algorithms

## Please write a summary of the paper [from 3 to 6 sentences].
The work generalizes existing algorithms for communication-efficient matrix multiplication. It also introduces a novel algorithm for 2.5D LU decomposition to minimize communication. The esults show that the 2.5D matrix multiplication and LU algorithms scale more efficiently
than baseline 2D algorithms.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
- The work shows strong scaling results up to 131072 nodes.
- The 2.5D LU algorithm achieves lower bandwidth cost by a factor of c^(1/2) compared to standard 2D LU algorithms, attaining the communication lower bounds.
- The paper provides a comprehensive analysis of both theoretical bounds and practical implementations

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
- The improvements in communication efficiency come at the cost of increased memory usage.
- The applicability of the techniques to sparse matrices or other problem domains is not extensively explored.
- The implementation and performance results are mainly presented for specific architectures


## Please provide a question for in-class discussion.
Can application libraries adopt the 2.5D algorithms such that practitioners can directly use them?

## Please provide a question for in-class discussion.
How might the principles of 2.5D algorithms for matrix operations be adapted to other important computational problems in scientific computing?


