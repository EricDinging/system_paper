# [GLUEFL: RECONCILING CLIENT SAMPLING AND MODEL MASKING FOR BANDWIDTH EFFICIENT FEDERATED LEARNING](https://arxiv.org/pdf/2212.01523.pdf)
## Problem
- Communication efficiency

## Backgrounds
- User sampling to reduce stragglers
- Masking: client side masking, server side masking
## Challenges
- Sampling leads to inefficient masking 
## Observations

## Ideas
- use sticky sampling
    - with a weighted central aggregation scheme to ensure that model updates remain unbiased
- gradual mask shifting strategy to reduce synchronization for a newly selected clients 
## Contribution

## Methods

## Results
- preserves unbiasedness of updates and convergence

## Application

## Limitation

## Questions