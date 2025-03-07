# Demystifying Map Space Exploration for NPUs

## Please write a summary of the paper [from 3 to 6 sentences].

The paper covers both heuristics and learning-based optimization approaches, analyze their behavior, and learn from their best traits.
The paper proposes warm start to trim the search space through using a mapping replay buffer. It also proposes sparsity-aware search method that can generate a mapping that generalizes to different sparsity levels.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
- The paper introduces novel methods to help accelerate MSE, which I think is a great idea based on the iterative nature of the ML workloads.
- This paper provides a holistic framework for outsiders to learn the design space.
- The paper has detailed workload input-output size breakdowns for readers to understand the requirement.

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
- The paper does not provide an end-to-end example of running a workloads on a specific DPU
- The paper only includes two metrics as objectives: energy and latency. There could be other metrics such as throughput and utilization to explore.
- The workloads discussed are limited, not including LLMs or diffusion models.

## Please provide a question for in-class discussion.
The work is insightful and covers different dimensions of MSE problem. I wonder whether the analysis can be applied to mapping workloads to heterogeneous hardware other than within one TPU, or a combination of both.

## Please provide a question for in-class discussion.
What component should be responsible for executing MSE result, hardware scheduling logic or compiler, or both?


