# Accelerating Multi-GPU Embedding Retrieval with PGAS-Style Communication for Deep Learning Recommendation Systems

## Please write a summary of the paper [from 3 to 6 sentences].
This paper uses PGAS communication method to optimize sparse input multi-GPU embedding retrieval in DLRM models. The method achieves better computation and communication overlap, balanced network usage and reduced overhead. The system achieves 2.63x speedup over NCCL collectives.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
- The approach achieves 2.63x speedup over the speed-of-the-art, which is impressive.
- The work bridges the gap between theoretical benefits of PGAS communication and practical deployments of DL frameworks (PyTorch).

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
- The paper does not include the discussion of NVSHMEM, which is a PGAS style communication library.
- Whether the approach can scale to multiple GPUs across nodes is not discussed.
- The authors do not provide a detailed analysis of the time components in the NCCL baseline.

## Please provide a question for in-class discussion.
Do you think the approach can scale well to multiple GPUs across nodes?

## Please provide a question for in-class discussion.
Is it possible to adopt this method in training pipeline, such as expert layers which have sparse communication patterns?



