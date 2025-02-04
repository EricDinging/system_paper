# Chimera: Efficiently Training Large-Scale Neural Networks with Bidirectional Pipelines

## Summary
Chimera is a novel pipeline-parallelism framework for distributed LLM training. It uses bi-directional pipelines, and computation-communication overlap. Chimera causes less bubbles in pipeline (higher pipeline utilization) as SOTA and the same peak activation memory consumption than SOTA frameworks, achieving end-to-end performance improvements between 1.38x-2.34x.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
1. This work conducts large scale simulation on 2048 nodes, and show strong empirical results.
2. The design is scalable to more micro-batches and more pipelines.
3. The paper has very clear illustrations for understanding the benefit (less bubbles and less peak memory usage).

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
1. The framework can be only applied to repetitive models like transformers.
2. Framework users need to search the parameters themselves. It would nice to integrate the searching process into the frameworks.


## Please provide a question for in-class discussion.
How do users decide how many layers should be placed in one GPU?

## Please provide a question for in-class discussion.
How do you think the researchers come up with the idea? I think this process involves a lot of drawing on the whiteboard.

