# [Vulcan: Automatic Query Planning for Live ML Analytics](https://yiwenzhang92.github.io/assets/docs/vulcan-nsdi24.pdf)
## Problem
- live ML analytics. How to perform automatic query planning, along with adapting to runtime dynamics
- Find query plans that optimize latency and accuracy, while minimizing the network and compute resource consumption
- An online adaptation technique is needed for faster convergence and lower cost
## Challenges

## Backgrounds
- live ML
    - Deployed across heterogeneous infrastructure
    - latency requirement besides accuracy
    - Query planning
        - Construct the pipeline by select a series of operators and ordering them
        - Determine the physical placement of pipeline operators across infrastructure tiers
        - Select configurations of the pipeline operators to optimize for query performance
## Observations

## Ideas

## Contribution

## Methods
- Define a metric to quantify each operator in the pipeline, converting the complexity of filter ordering from exponential to linear
- Select the ordering of the filter
    - Based on a metric defined by precision and recall
    - Treating a set of filters as a bulk filter to prune search space
- Placement
    - Reducing search cost by reusing intermediate results from pipeline runs
    - Early pruning unpromising placement choices
- Identifies components of ML pipelines that are independent of placement
- Efficiently explores the best combination of configuration knobs using Bayesian Optimization
    - BO is a methodology for optimizing expensive objective functions
- Adapt quickly to dynamic changes in data and resources
    - Monitor utility change to detect runtime dynamics
    - Leverage prior knowledge during profiling
## Results

## Application

## Limitation

## Questions