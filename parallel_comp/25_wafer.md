# Near-Optimal Wafer-Scale Reduce

## Please write a summary of the paper [from 3 to 6 sentences].
This work performs an in-depth exploration of communication collectives on the Cerebras WSE. It introduces a streamlined model to design algorithms for the hardware, and demonstrates that this model accurately predicts performance on the WSE. Leveraging the multi-cast feature of the WSE specialized collectives outperform previous algorithms by up to 3.27×.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
1. The work is the first to benchmark different collectives on WSE.
2. The work consider timing issues in distributed system.
3. It proposes a novel framework to help programmers develop collectives for a new architecture.


## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
1. 1D allreduce discussion is limited to ring algorithm.
2. The authors configure the routers such that at a given cycle they accept wavelets only from a single direction. This seems sub-optimal.
3. The paper does not give a concrete analysis of the architecture.

## Please provide a question for in-class discussion.
Is the communication between PE and router full duplex?

## Please provide a question for in-class discussion.
Is there a need to model the compuation cost of collectives for WSE?



