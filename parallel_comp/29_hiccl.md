# HiCCL: A Hierarchical Collective Communication Library

## Please write a summary of the paper [from 3 to 6 sentences].
HiCCL is a collective communication library that is optimized for hierarchical and heterogeneous networks. HiCCL compose local collective operations which use ring or tree to execute global collective operation using three primitives: multi-cast, reduce, and fence. It outperforms vendor-specific collective libraries while providing portability across machines.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
1. HiCCL provides performance portability across systems of different shapes and sizes and of different vendors.
2. HiCCL moves less data on higher network hierarchy, reducing contention.
3. HiCCL is shown to outperform vendor specific library across multiple hardwares.

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
1. Some of the optimizations like striping and pipelining are already performed in baselines like NCCL.
2. HiCCL relies on the assumption that network is hierarchical. However, HiCCL may not outperform other libraries when running on full-bisection network.
3. The evaluation section does not specify the protocols used for different systems, which could impact the performace.

## Please provide a question for in-class discussion.
Would hierarchical collectives introduce network imbalances with some nodes producing more traffic than others?

## Please provide a question for in-class discussion.
Why does NCCL scale better than HiCCL?


