# [Carousel: Scalable Traffic Shaping at End Hosts](https://saeed.github.io/files/carousel-sigcomm17.pdf)
## Problem
- Shape traffic based on the priority of the application
during times of congestion
- Accurate shaping to a target rate is important for efficient network operation
- Deep queue -> reduce packet loss, also increase latency
- Network isolation between VMs on the same host
- Existing strategy either does not perform well under bursty flows or consume too much compute
## Challenges

## Observations

## Ideas
- Pacing between packets within one flow
- Rate limiting on aggregated flows

## Contribution

## Methods
- A single queue shaper using time as the basis for scheduling
- Coupling actual packet transmission to the freeing of resources in higher layers
- Each shaper runs on a separate CPU core, which could be as few as one CPU
- Design principles
    - Work compatibly with higher level congestion control mechanisms such as TCP.
    - Use CPU and memory effciently

## Results

## Application

## Limitation

## Questions