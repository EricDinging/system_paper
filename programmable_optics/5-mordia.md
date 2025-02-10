# Integrating Microsecond Circuit Switching into the Data Center

## Summary
Mordia is a datacenter control plane based on fast circuit switches and a low-latency circuit scheduling approach. The scheduling approach, called Traffic Matrix Scheduling (TMS), computes short-term schedules using short-term traffic demand and quickly multiplexes the circuit across a set of end points, instead of observing long-lived traffic demand. To remain synchronized with OCS, a controller notifies the ToR switch with circuit schedules.

## Pros
1. The end-to-end reconfiguration time is 2–3 orders of magnitude smaller than previous approaches.
2. The control plane is decoupled from switch implementation.
3. The paper provides end-to-end measurement and performance breakdown.

## Cons
1. The paper does not address issues in other layers of the network stack. For example, TCP might not be able to fully utilize the link bandwidth within such a short switching window.
2. Mordia prototype requires wavelength multiplexing, restricting scalability.

## Discussion
1. What's the proper way to perform demand estimation?