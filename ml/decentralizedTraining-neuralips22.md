# [Decentralized Training of Foundation Models in Heterogeneous Environments](https://proceedings.neurips.cc/paper_files/paper/2022/file/a37d615b61f999a5fa276adb14643476-Paper-Conference.pdf)
## Problem
- Large compute to train FM
- Existing framework tailor to fast, homogenous data center networks
- Decentralized training focus solely on data parallelism, insufficient for FM whose parameters exceed the capacity of a single device
## Challenges
- Assign tasks, micro-batch and a subset of layers, to a collection of devices connected via heterogeneous, slow networks
## Observations

## Ideas
- In a decentralized environment, the training procedure is communication-bounded. The scheduling problem is to accelerate the communication procedure by allocating tasklets that require high communication volumes between them to devices with faster connections.
- Scheduling in Heterogeneous Environments, a bi-level scheduling algorithm
    - Extended balanced graph partition problem
- Searching via hybrid genetic algorithm

## Contribution

## Methods
- Kernighan-Lin Algorithm
## Results

## Application

## Limitation
- Fault tolerance
## Questions