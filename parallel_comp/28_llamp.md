# LLAMP: Assessing Network Latency Tolerance of HPC Applications with Linear Programming

## Please write a summary of the paper [from 3 to 6 sentences].
The work points out the challenge HPC workloads are facing nowadays that high latency from network affect application performance. The work introduces LLAMP, a tool chain based on linear programming and LogGPS that could analyze the network latency and application tolerance for HPC workloads. The researchers also developed a latency injector to emulate flow-level latency with an error margin of less than 2%.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
- The work points out the interesting tradeoffs between high bandwidth and low latency due to FEC requirement of high bandwidth links.
- The predictor does not require hardware environment which might be costly.
- The work analyzes different collective algorithms' impact on the workload tolerance on network latency.

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
- The paper does not mention alpha-beta model and its relation to the paper's formulation.
- The uniform modelling of switch latency does not take into account the queueing delay, which could be different across different switches.
- The solver could take thousands of seconds to solve.


## Please provide a question for in-class discussion.
What actions could programers do after performing the latency tolerance analysis to accelerate workload?

## Please provide a question for in-class discussion.
Is it realistic to model the network latency as only a single value in the HPC cluster?
