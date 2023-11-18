# [Gaia: Geo-Distributed Machine Learning Approaching LAN Speeds](https://www.usenix.org/system/files/conference/nsdi17/nsdi17-hsieh.pdf)
## Problem
- Infeasible to move globally-generated data to a centralized data center
- Communicating over WANs can significantly degrade ML system performance

## Challenges
- Minimize communication
- General enough to be applicable to a wide variety of ML algorithms, without requiring any algorithm changes

## Observations

## Ideas
- Geo-distributed ML system that employs an intelligent communication mechansim over WANs
- Gaia
    - Decouples the communication within a data center from the communication between data centers
    - ML synchronization model, Approximate Synchronous Parallel, bounding how inaccurate a parameter can be, aggregating insignificant partial updates
    - Provides the ML worker machines with a distributed global shared memory abstraction
    - Maintain an approximately-correct copy of the global ML model within each data center

## Methods

## Results

## Application

## Limitation

## Questions