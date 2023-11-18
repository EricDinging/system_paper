# [EC-Cache: Load-Balanced, Low-Latency Cluster Caching with Online Erasure Coding](https://www.usenix.org/conference/osdi16/technical-sessions/presentation/rashmi)
## Problem
- Data-intensive clusters and object stores are increasingly relying on in-memory object caching to meet the I/O performance demands. These systems routinely face the challenges of popularity skew, background load imbal- ance, and server failures, which result in severe load im- balance across servers and degraded I/O performance.
## Challenges
- Popularity skew
- Background load balance across infrastructure
## Observations
- the design of in- memory solutions boils down to maximizing the number of requests that can be efficiently served from memory
    - determine which one to cache and which one to evict
    - increase the in-memory capacity (sampling and compression)
    - Ensuring good I/O performance for the cached data in the presence of skewed popularity, background load imbalance, and failures
- Data popularity is heavily-skewed -> load imbalance in the data center
    - Over-provisioning
    - Adversely affect the IO performance

## Ideas
- Selective repeat -> fall short of load balancing and I/O performance due to limited memory
- Erasure coding, toward load balancing and improving I/O performance in cluster caches
    - Reconstruction using parities incurs huge bandwidth overheads
## Methods
- EC-Cache is a load-balanced, low latency cluster cache that uses online erasure coding to overcome the limitations of selective replication
-  EC-Cache divides individual objects into k splits and creates r additional parity splits. Read requests to an object are served by reading any k of the (k+r) splits and decoding them to recover the desired object
    - Spreading the load of read requests across both data and parity splits results in better load balancing under skewed popularity
    - Better IO performance
- Late binding, reading k + delta from k + r splits
    - Resilient to stragglers
- Reed-Solomon code
## Results

## Application
- Caching layer on top of object stores
## Limitation
- offers advantages only for objects greater than 1 MB due to the overhead of creating K + delta parallel TCP connections for each read
- Suitable for immutable objects. Workloads with frequent, in-place updates are not suitable for EC-Cache because they would require updating all the parity splits of the updated objects

## Questions