# [ServiceRouter: Hyperscale and Minimal Cost Service Mesh at Meta](https://www.usenix.org/system/files/osdi23-saokar.pdf)
## Problem
- Datacenter applications are often structured as many interconnected microservices
- Service mesh has become a popular approach to route RPC traffic among services
- Present Meta's global service mesh: ServiceRouter
## Challenges
- Designed for hyperscale, use millions of L7 routers to route tens of billions of requests per second across tens of thousands of srvices

## Observations

## Ideas
- Use remote proxies to route 1% of RPC requests, which is the common approach
- Employ a routing library that is directly linked into service executables to route the remaining 99% directly from clients to servers

## Results
- Significantly reduces the hardware costs, no need for proxies
- Provides built-in support for sharded services, which account for 68% of RPC requests at meta
- Introduce the concept of locality rings to simultaneously minimize RPC latency and balance load across geo-distributed datacenter regions

## Application

## Questions