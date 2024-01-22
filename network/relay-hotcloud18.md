# [To Relay or Not to Relay for Inter-Cloud Transfers?](https://www.usenix.org/system/files/conference/hotcloud18/hotcloud18-paper-lai.pdf)
## Problem
- Geo-distributed analytics
    - across geo-distributed datacenters
    - large data transfers across WAN
    - high spatial and temporal bandwidth variation
## Challenges

## Backgrounds

## Observations
- WAN bandwidth between close datacenters can be 12x more than between distant regions
    - Artificial measurements, only one TCP connection
    - Should be measured as the aggregate bandwidth of multiple TCP connections
## Ideas
- Naive: Relaying inter-datacenter transfers via detours
    - Not solid due to artificial measurements of prior works
## Contribution

## Methods
- Inter-cloud WAN measurements
    - iperf3 to measure bw
    - ping (ICMP) and hping3 (TCP) to measure the RTT
    - Enlarge TCP window size of 7MB, setting up multiple TCP connections per VM
## Results
- Show that there is
    - Per-flow rate limiting
    - available WAN bandwidth is homogenous at the VM level and capped per-VM
    - Bandwidth is stable over periods of time
    - Contention occurs at VMs instead of inter-datacenter links
    - Not much scope for latency optimizations
- WAN bandwidth is often homogeneous (spatially and temporally)
- Aggregate outbound and inbound rates are limited by the VM rate cap
- WAN latency varies greatly between different regions
## Application
- Relay may not be helpful for higher network throughput because of VM rate cap
- Use multiple TCP connections
## Limitation

## Questions