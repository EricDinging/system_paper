# Jupiter Rising: A Decade of Clos Topologies and Centralized Control in Google’s Datacenter Network

## Summary
This paper shares Google's engineering experience behind ten years of production datacenter networks. It shows the general trend of moving towards centralized control plane for ease of management and high bisection bandwidth.

## Pros
1. The paper provides an interesting observation that storage placement and job scheduling have little locality in our cluster traffic for fault tolerance and power management purposes, placing extra burden on networks. 


## Cons
1. Due to the paper's nature as an industry-track paper, some of the design choices and operation details are not clearly illustrated or explained.