# The Landscape of GPU-Centric Communication

## Please write a summary of the paper [from 3 to 6 sentences].
This survey paper covers the GPU-centric networking technologies. It categorizes intra-node and inter-node GPU communication through four dimensions: registration, data path, API endpoints, and trigger. The survey paper also discusses hardware vendor technologies including: (1) host physical memory locking, (2) Unified Virtual Addressing (UVA) and Unified Virtual Memory (UVM), and (3) GPU-direct technologies. The authors conclude that CPU-free communication scheme is promising, which could potentially remove latency related to CPU and improve instruction level parallelism. However, memory consistency remains a problem.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
- This survey paper has illustrative tables and plots, helping readers understand the communication models.
- The paper offers a full-stack view of GPU communication, from hardware vendor library to application-level library such as PyTorch.
- The paper presents a general trend moving from CPU-centric communication towards GPU-centric communication through compelling arguments.
- The paper tries to consider networking stack from all vendors, including AMD and Intel.

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
- The paper does not have experiments to show performance difference of different communication scheme or different technologies.
- The paper does not offer examples showcasing the memory consistency issues in GPU-initiated OpenSHMEM communication.
- The paper could talk more about the application level benefit of GPU-centric networking.

## Please provide a question for in-class discussion.
Where is the page table stored when using UVA?

## Please provide a question for in-class discussion.
If GPU is responsible for all communication, do the communication protocols have congestion control and reliability guarantees? If so, is it efficient to implement these logic using GPU?


PCIe
NVLink

GPU direct async: pre-register?

How does NCCL implement communication and computation in one kernel?

Address in NVLINK network

What is the infiniband/roce protocol details

UCX?
MSCCL
