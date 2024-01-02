# [Arboretum: A Planner for Large-Scale Federated Analytics with Differential Privacy](https://haeberlen.cis.upenn.edu/papers/arboretum-sosp2023.pdf)
## Problem
- Due to the distributed nature of FA, FA solutions support only a limited class of queries 
## Challenges
- Scalability of DP FA, the computational cosst at scale would be astronomical
    - Exponential mechansim, for categorical querying, require a lot of computation
## Observations
- Devices are also resources. Break query plans into small, bite-size pieces that are each within the means of a small device
- Possible to build a query planner for federated analytics that automatically finds a very good plan for most queries
## Ideas
- Use the device with the computation
    - Organic scaling: adding devices increases both the demand for resources and supply (CDN, decentralized system)
- Design space has a fairly regular structure
## Contribution
- FA system, a query planner, that can efficiently answer a broader range of queries, including cateogorical queries
    - Automatically optimizing query plans to find highly efficient ways to answer each query
    - Include the participant devices in the computation
## Methods
- DP
- Multi-party computation
- Homomorphic encryption FHE

- Thread model
    - Occasional Byzantine: the aggregator should not be fully trusted
    - Mostly Correct

## Results

## Application

## Limitation

## Questions