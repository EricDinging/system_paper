# [Sparrow: Distributed, Low Latency Scheduling](https://people.eecs.berkeley.edu/~matei/papers/2013/sosp_sparrow.pdf)
## Problem
- Data analytics clusters are running ever shorter
and higher-fanout jobs

## Challenges
- When tasks run in
hundreds of milliseconds, scheduling decisions must be
made at very high throughput
- High throughput, low latency, high availability
- The key challenge with a decentralized design is providing response times comparable
to those provided by a centralized scheduler, given that
concurrently operating schedulers may make conflicting
scheduling decisions
## Observations

## Ideas
- the power of two choices load balancing technique
- Batch sampling
- Late binding
- Policies and constraints

## Methods
- Sparrow provides fine-grained task scheduling, which
is complementary to the functionality provided by cluster resource managers. Sparrow does not launch new
processes for each task; instead, Sparrow assumes that
a long-running executor process is already running on
each worker machine for each framework, so that Sparrow need only send a short task description (rather than
a large binary) when a task is launched.

## Results
-  a decentralized, randomized sampling approach provides near-optimal performance while avoiding the throughput and availability
limitations of a centralized design

## Application

## Limitation

## Questions