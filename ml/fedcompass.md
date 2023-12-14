# [FedCompass: Efficient Cross-Silo Federated Learning on Heterogeneous Client Devices Using a Computing Power-Aware Scheduler](https://arxiv.org/pdf/2309.14675.pdf)
## Problem
- FL empowers the training of more robust and generalized models while preserving the privacy of client data
- Disparity of computing power
among participating client devices leads to significant variations in local training times
## Challenges

## Observations

## Ideas
- Focus on improving the performance in cross-silo FL settings
- Computing power aware scheduler to reduce client local model staleness and FL efficiency in cross-silo settings
- Compass assesses the computing power of individual clients based on their previous response times and dynamically assigns varying numbers of local training steps
to ensure that a group of clients can complete local training almost simultaneously
- Group aggregation leads to less global update
frequency and reduced local model staleness, thus mitigating client drift and improving the performance on non-IID heterogeneous data.
## Contribution

## Methods

## Results

## Application

## Limitation

## Questions