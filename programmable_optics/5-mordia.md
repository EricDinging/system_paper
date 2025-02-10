# Integrating Microsecond Circuit Switching into the Data Center

## Summary
Mordia is a datacenter control plane based on fast circuit switches and a low-latency circuit scheduling approach. The scheduling approach, called Traffic Matrix Scheduling (TMS), computes short-term schedules using short-term traffic demand and quickly multiplexes the circuit across a set of end points, instead of relying on long-lived conditions.  

## Pros
1. end-to-end reconfiguration time 2–3 orders of magnitude smaller than previous approaches.
2. Control plane is decoupled from switch

## Cons
1. Does not address the issues in other layers of the network stack. For example, TCP might not be able to fully utilize the link bandwidth within such a short switching window.

## Discussion
1. What's the proper way to perform demand estimation?