# faimGraph: High Performance Management of Fully-Dynamic Graphs Under Tight Memory Constraints on the GPU

## Please write a summary of the paper [from 3 to 6 sentences].
faimGraph is a memory management system for graph data on GPU. It allows dynamic graph data modification (vertex insertion and deletion, edge insertion and deletion). faimGraph is highly performant, capable of performing more than 300 million adjacency queries and millions of vertex updates per second. 

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
1. The work introduces a novel idea, implementing dynamic memory management on GPUs.
2. The work solves several challenges: minimizing memory fragmentation on GPUs, decreasing memory requirement, and allowing dynamic graph data insertion and deletions.
3. The paper presents both microbenchmarks and macrobenchmarks.

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
1. The paper claims applications show an efficient memory access pattern and better caching behavior using faimGraph. The reasoning behind is not clear.
2. The paper does not discuss GPU caching on the performance impact of faimGraph. Could faimGraph gain performance through aligning data structure with cache line sizes?


## Please provide a question for in-class discussion.
How does the GPU-based memory management system compare with CPU-based memory mamangement system? Would it be beneficial to have CPU threads (with more control logic performance) managing the data structure and let GPU threads read and write the data?

## Please provide a question for in-class discussion.
What could be the worst-case performance of the system, imaging all GPU threads are accessing the graph data?


