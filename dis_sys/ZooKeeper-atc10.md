# [ZooKeeper: Wait-free coordination for Internet-scale systems](https://www.usenix.org/legacy/event/atc10/tech/full_papers/Hunt.pdf)
## Problem
- Dynamic configuration of distributed system
-  Group membership and leader election are also common in distributed systems: often processes need to know which other processes are alive and what those processes are in charge of
## Challenges
- Blocking
primitives for a coordination service can cause, among
other problems, slow or faulty clients to impact negatively the performance of faster clients.

## Observations

## Ideas
- Simple and high performance kernel for building more complex coordination primitives at the client
- It incorporates elements from group messaging,
shared registers, and distributed lock services in a replicated, centralized service
- When designing our coordination service, we moved
away from implementing specific primitives on the
server side, and instead we opted for exposing an API
that enables application developers to implement their
own primitives

## Methods
- Wait free shared registers
- Per client guarantee of FIFO execution of requests, and linearizability for all requests that change the ZooKeeper state
- Implements an API that manipulates simple waitfree data objects organized hierarchically as in file systems
- Leader-based atomic broadcast protocol
- ZooKeeper uses a watch
mechanism to enable clients to cache data without managing the client cache directly
## Results

## Application

## Limitation

## Questions