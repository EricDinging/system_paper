# [Network Load Balancing with In-network Reordering Support for RDMA](https://dl.acm.org/doi/pdf/10.1145/3603269.3604849)
## Problem
- RDMA does not work well with existing load balancing alg because of its traffic flow characteristics and assumption of in-order packet delivery
## Challenges

## Observations

## Ideas
- Use a programmable switch to perform fine granularity rerouting
- Mask the effect of out-of-order packet arrivals

## Results
- Evaluations show that ConWeave can achieve up to 42.3% and 66.8% improvement for average and 99-percentile
FCT

## Application

## Limitation

## Questions