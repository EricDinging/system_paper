# Deepseek technical report
## Ideas
Multi-token generation

Clever EP routing

Mixed precision training

## Questions
1. How EP work? Is each sequence or token in a batch mapped to different experts?

    Each token will be matched to a different expert.
2. What are the affinity scores

    Probability of one token being mapped to an expert
3. Full computation-communication overlap?

    Asynchronous data transfers
    
    Multiple cuda streams
4. Token dropping?
5. cross-node expert parallelism

    Results in an inefficient computation-to-communication ratio of approximately 1:1

7. Bandwidth comparison

    nvlink1.0 level
8. Parallelism degree is not uniform. 

    1TP -> 4TP

10. Prefilling and decoding using different sets of nodes?

    DistServe: prefilling and decoding disaggregation.
    Does it mean it is important to work on communication for kv cache state transfer?
11. Why you can allocate smaller amount of SMs?
12. Reduce operation for all-to-all combine?
13. Workload placement
14. Auxiliary loss free
15. How is RL performed