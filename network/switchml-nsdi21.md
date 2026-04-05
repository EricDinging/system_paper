# Scaling Distributed Machine Learning with In-Network Aggregation

## Summary
Accelerate distributed parallel training by designing a communication primitive that uses a programmable switch dataplane to execute a key step of training process.

## Challenges
1. Compute and memory on switch is limited
2. Switch operates on integer values
3. Pattern is all-to-all

## Insights
1. Aggregation can be parallelized and pipelined
2. Aggregation for SGD can be applied separately on different portions of input data, tolerating slight loss. Retransmission mechanism is driven solely by end hosts, ensuring that workers operate in lock-step
3. Scale the floating points to fixed-point

## Pros
1. In-network aggregation in an Ethernet network