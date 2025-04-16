# Harnessing Integrated CPU-GPU System Memory for HPC: a first look into Grace Hopper

## Please write a summary of the paper [from 3 to 6 sentences].
The work discusses the integrated CPU-GPU system memory of the Grace Hopper system. It compares two memory management strategies: system-allocated memory and CUDA-managed memory. And it evaluates two strategies' performance on six HPC applications. The results show that the system-allocated memory can be beneficial for most use cases.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
1. The work shows the distinction between system memory and managemd memory.
2. The evaluation breaks down the time spent in individual stages of the workload.
3. The results are very helpful for a broader community to understand NVIDIA's system.

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
1. The work studies the behavior of Grace Hopper system memory using only HPC workloads, which might not be useful for ML workloads.
2. The evaluation does not have cache-miss ang page-miss plots in those workloads.
3. Some experiments are not holistic. The experiment studying the system page size influence on application performance only studies two configurations.

## Please provide a question for in-class discussion.
If the application has a very high spatial-locality, would managed memory outperform system memory?

## Please provide a question for in-class discussion.
What will be the system's behavior if there are multiple GPUs reading the same data? Will the conclusion still hold true?
