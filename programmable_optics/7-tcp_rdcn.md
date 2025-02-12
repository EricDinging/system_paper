# Adapting TCP for Reconfigurable Datacenter Networks
## Summary
The paper addresses a very pressing issue that, as reconfigurable networks become faster and faster, the ramp-up delay by the TCP stack becomes more and more prominant. To solve this issue, packets are pre-buffered in ToR switch virtual output queues before the circuits are constructed. Also, congestion window size is dynamically configured through explicit circuit state feedback. Using an in-house reconfigurable network simulator, the researchers show their work could increase circuit utilization by 1.91x with only 1.20x in tail latency.

## Pros
1. The paper is well-motivated. The motivation behind changing TCP is straight-forward.


## Cons
1. Ramp-up time may exceed circuit downtime, meaning the circuit cannot be fully utilized even with pre-buffered traffic.

## Interesting points
1. Segragating elephant flows and mice flows and routing them over different network are sub-optimal.