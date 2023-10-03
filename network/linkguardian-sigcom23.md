#[Masking Corruption Packet Losses in Datacenter Networks with Link-local Retransmission](https://dl.acm.org/doi/pdf/10.1145/3603269.3604853)

## Problem
- Packet loss due to link corruption in large warehouse-scale datacenters
- All the corrupting links cannot be disabled due to capacity constraints
## Challenges

## Observations
- Feasible to implement link-local retransmission at sub-RTT timescales to completely mask corruption packet losses
## Ideas
- Keep packet buffer requirement low
- Recover from tail packet losses without employing timeouts
- Preserve packet ordering

## Results
- Reduce the loss rate by up to 6 orders of magnitude while incurring only 8% reduction in effective link speed

## Application

## Limitation

## Questions