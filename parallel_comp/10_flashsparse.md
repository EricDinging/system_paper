# FlashSparse: Minimizing Computation Redundancy for Fast Sparse Matrix Multiplications on Tensor Cores

## Please write a summary of the paper [from 3 to 6 sentences].
This paper introduces FlashSparse, a method to enhance sparse matrix multiplication efficiency using tensor core unit architecture. Using a swap-and-transponse matrix multiplication strategy, FlashSparse minimizes the sparse granularity for SpMM and SDDMM on TCUs to boost compute efficiency. Also, FlashSparse uses memory-efficient thread mapping strategy for coalesced data access and a sparse matrix storage format to save memory. Evaluation shows that FlashSparse sets a new state-of-the-art.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
- This paper utilizes specific hardware architectures for performance enhancement.
- The performance improvement compared to the baseline is impressive.
- FlashSparse does not impact model accuracy.

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
- The figure labels are not legible.
- The evaluations are only performed on two machines
- The framework is limited to architectures with TCUs. 

## Please provide a question for in-class discussion.
- Would it be feasible to integrate the ideas from the two papers we read today to form a higher level framework that could be applied to any kinds of GPUs?

## Please provide a question for in-class discussion.
- If we need multiple GPUs for graph application, can we still FlashSparse?


