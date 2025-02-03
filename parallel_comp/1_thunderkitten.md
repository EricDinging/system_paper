# ThunderKittens: Simple, Fast, and Adorable AI Kernels

## Please write a summary of the paper [from 3 to 6 sentences].
The paper proposes ThunderKitten (TK): a light-weight, easy-to-use, and yet very powerful GPU kernel framework. TK relies on three level of abstraction: (1) warp-level tile data structure and logical data to memory mapping for low level acceleration and bank-conflict minimization, (2) block-level pipeline and worker-consumer model for memory and computation overlapping, and (3) grid-level scheduling to improve cache hit rates. Kernels written in TK achieves similar performance as SOTA kernel frameworks which are more difficult to program.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
1. TK achieves impressive results yet remain relatively simple to use.
2. TK has good performance without breaking abstraction. It can work idealy on any Nvidia hardware with good performance without requiring users to do low-level programming.
3. TK can be applied to a wide range of ML operations.

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].

1. The paper does not explain the relationship between thread block and SM and its design decision very well. It seems to assume one thread block runs on one SM but in reality multiple thread blocks can run on one SM at the same time.
2. The reasoning behind using tiles as basic data structures is not clear to me.
3. TK does not describe in details about its grid scheduling policy.

## Please provide a question for in-class discussion.
TK is useful to accelerate workloads running on one GPU. In distributed application, communication is one of the main bottlenecks. Some GPU resources (SM, memory) will be used for communication. Do you think TK can be extended for those applications?

## Please provide a question for in-class discussion.
How does TK know what is the optimal configurations (logical data to physical memory mapping, number of load/store stages) for certain applications running on certain hardware?

