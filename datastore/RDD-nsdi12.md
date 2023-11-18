# [Resilient Distributed Datasets: A Fault-Tolerant Abstraction for In-Memory Cluster Computing](https://www.usenix.org/system/files/conference/nsdi12/nsdi12-final138.pdf)
## Problem
- distributed framework write partial results to a external stable storage system, overhead
- Memory reuse framework has a limited problem scope

## Challenges
- fault tolerance without incuring copying data over limited bandwidth network

## Observations

## Ideas
- Store lineage, operations on the data instead of the data itself

## Methods

## Results
-  lets programmers perform in-memory computations on large clusters in a
fault-tolerant manner
## Application
- Course-grained operation on dataset

## Limitation
- make asynchronous fine-grained updates to shared states

## Questions