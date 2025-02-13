# Distributed Matrix-based Sampling for Graph Neural Network Training

## Please write a summary of the paper [from 3 to 6 sentences].
This paper proposes a method to reduce communication in the sampling step for GNN model training. It uses matrix-based bulk sampling that samples multiple minibatches at once in a distributed manner without the need of communication. It shows strong scaling result for different sampling algorithms.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
- Experimental results show significant speedups over existing methods, with up to 2.5× faster performance than Quiver and 8.46× speedup on 128 GPUs for certain datasets.

- The approach is implemented in an end-to-end training pipeline.


## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
- The paper might benefit from theoretical analysis explaining why the matrix-based approach works well and its potential limitations.

- A more detailed analysis of how the sampling method affects model accuracy is missing.




## Please provide a question for in-class discussion.
Will the sampling algorithm affect training accuracy?

## Please provide a question for in-class discussion.
How might the matrix-based bulk sampling approach be adapted for different types of graph structures?


