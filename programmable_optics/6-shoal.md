# Shoal: A Network Architecture for Disaggregated Racks

## Summary
Shoal is a power-efficient and performant network design for disaggregated racks. To achieve nano-second switching, Shoal does not rely on a centralized controller, and requires each rack to send traffic according to a static schedule. Its congestion control ensures fairness and bounded worst-case performance. Shoal achieves 71% lower power and comparable or higher performance than today’s network designs.

## Pros
1. Shoal uses coordination-free routing with latency guarantees, obviating the need for a central controller.
2. Shoal improves the transport layer using backpressure-based congestion control for efficient multi-pathing routing.

## Cons
1. Shoal is limited to disaggregated network architecture.