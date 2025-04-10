# Efficient Algorithms for Monte Carlo Particle Transport on AI Accelerator Hardware

## Please write a summary of the paper [from 3 to 6 sentences].
This work design implement Monte Carlo partical transport algorithm on WSE. The proposed algorithm minimizes communication costs and balances load. The end-to-end performance gain is 130x over A100.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
1. The target workload is important and yet not widely studied on WSE architecture, which is based on a highly irregular stochastic algorithm that does not involve matrix operations.
2. The paper provides a systematic comparison between A100 and Cerebras architecture.
3. The solution leverages random number generation feature in Cerebras architecture to boost lookup kernel performance by over 65%.

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
1. The comparison with A100 might be unfair, since A100 chip area might be smaller than Cerebras chip.
2. The paper should compare Cerebras solution with multi-GPU solution.
3. The paper could better illustrate the communication pattern using traffic matrix.

## Please provide a question for in-class discussion.
What architecture feature is the most helpful for accelerating MC particle transport on WSE compared to GPUs?

## Please provide a question for in-class discussion.
Is it necessary to develop a programming framework for WSE to simplify the communication algorithm design? If so, what would the interface look like?



