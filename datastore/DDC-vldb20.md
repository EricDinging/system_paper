# [Understanding the Effect of Data Center Resource Disaggregation on Production DBMSs](link)
## Problem
- Disaggregated data centers
    - Allow independent resource expansion
    - Prevent fragmentation and over-provisioning
    - Provides a near-infinite pool of any resource for any program 
    - Independent failures & independent allocation
- Disaggregated OS
    - LegoOS, splitkernel approach
## Challenges

## Backgrounds
- DBMS have complex software stacks, having a thorough understanding of their end-to-end performance in a DDC is therefore critical for the design, implementation and optimization of DBMSs in the future cloud architectures.
- Different query has unique access patterns
- Disaggregation expose many fundamental assumptions about memory accessing latency, buffer management, and paging strategies.
## Observations
- The cost of disaggregation is more observable than traditional distributed DBMS like Spark and Vertica.
- The main bottleneck in the DDC setting stems from memory stalls not compute parallelism
- Out-of-core execution are generally less sensitive to the degree of disaggregation than in-memory executions because of other bottlenecks
## Ideas

## Contribution

## Methods
- PostgreSQL: out-of-core
- MonetDB: in-memory
## Results
- Highlight the need for codesigning DDCs and DBMSs to avoid redundancy and mismatched policies
- resource disaggregation provides better and more stable performance than a single server for DBMSs when the execution reaches the memory limit in the server and they have to spill data to disk.
## Application

## Limitation

## Questions