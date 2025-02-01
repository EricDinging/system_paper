# Please write a summary of the paper [from 3 to 6 sentences].
The paper proposes ThunderKitten (TK): a light-weight, easy-to-use, and yet very powerful GPU kernel framework. TK relies on three level of abstraction: (1) warp-level tile data structure and logical data to memory mapping for low level acceleration and bank-conflict minimization, (2) block-level pipeline and worker-consumer model for memory and computation overlapping, and (3) grid-level scheduling to improve cache hit rates. 

simplifying the choice of memory layouts,
exploration of grid patterns for L2 reuse, and selection of occupancy and pipeline depth

# Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
1. Impressive result

# Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].

1. Does not explain the relation between thread block and SM well. Assume one thread block runs on one SM
2. Tile? and real tensor inputs
3. Reasoning behind the performance is not comprehensive: specialized instructions such as TMA and WGMMA?
4. Does not talk about grid scheduling a lot.

# Please provide a question for in-class discussion.
1. 

# Please provide a question for in-class discussion.



