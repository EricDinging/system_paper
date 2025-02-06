# LONG EXPOSURE: Accelerating Parameter-Efficient Fine-Tuning for LLMs under Shadowy Sparsity

## Please write a summary of the paper [from 3 to 6 sentences].
Long Exposure is a system design for parameter-efficient fine-tuning for LLMs. Long Exposure identifies sparse patterns tailored to each attention head, minimizing the computational redundancy or oversight. It is efficient in terms of both parameter and computation, demonstrating up to 2.49x speedup over state-of-the-art methods.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
1. The authors provide evaluation on two different GPU platforms, enhancing the credibility of the results.
2. The work points out the intrinsic sparsity within LLM fine-tuning.
3. The work use simple transformations to leverage memory coalescing, increasing computation throughput.

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
1. The performance enhancement is impressive. However, the work only gives empirical results in terms of model accuracy without formal proofs, even though the method could change the model output in addition to acceleration.
2. Prediction requires training a predictive model.

## Please provide a question for in-class discussion.
Is empirical result enough to convince people the feasibility of certain system optimization even if it will change the model output with the same input.

## Please provide a question for in-class discussion.
Does the prediction model scale to other model architecture?

