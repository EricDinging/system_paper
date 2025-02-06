# TORCHGT: A Holistic System for Large-scale Graph Transformer Training

## Please write a summary of the paper [from 3 to 6 sentences].
TorchGT is the first distributed training system for graph transformer models that could scale to large graphs with billions of edges. TorchGT uses local-global interleaved attention, cluster-aware graph parallelism, and elastic computation reformation for accelerating graph training. It achieves up to 62.7x speedup and near-linear scalability.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
1. TorchGT addresses both algorithmic and system-level challenges in training graph transformers.
2. The system demonstrates near-linear scalability, effectively distributing workloads across multiple devices without compromising performance.
3. Extensive experiments validate its efficiency, achieving significant speedups up to 62.7x.


## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
1. The elastic computation reformation may incur significant memory overheads when applied to extremely dense or irregular graphs.
2. The work does not provide enough insight into the trade-offs between computational efficiency and model accuracy.


## Please provide a question for in-class discussion.
Why does flash attention test accuracy drop after 10s in Figure 10?

## Please provide a question for in-class discussion.
How does TorchGT balance the trade-off between computational efficiency and model accuracy when scaling to extremely large graphs?