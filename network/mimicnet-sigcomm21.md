# [MimicNet: Fast Performance Estimates for Data Center Networks with Machine Learning](https://dl.acm.org/doi/pdf/10.1145/3452296.3472926)
## Problem
- Intractable data center innovations
- Hard to simulate data center workflows
    - Existing evaluation comprises orders of magnitude fewer devices and different network structures
## Challenges
- Quickly obtaining accurate performance estimates
- Arbitrary scale, extensions, and instrumentation
- Orders of magnitude faster results
- Tunable and high accuracy
## Observations

## Ideas
- Tool for fast performance estimation of at-scale data center networks
## Methods
- Runs a simulation of a small subset of the larger data center network
- Train a mimic using the generated data, fine tuning
    - Deep-learning-based internal models contained within each mimic
    - FLow-based feeder models that approximate the behavior of inter-cluster cross-traffic
- Predict the performance of an N cluster simulation
## Results

## Application

## Limitation
- Data center is built on a classic FatTree topology
- Congestion occurs primarily on fan-in
- Given host's connections are independently managed
## Questions