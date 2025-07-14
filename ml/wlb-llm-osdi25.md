# WLB-LLM: Workload-Balanced 4D Parallelism for Large Language Model Training

## Summary
- Analyze workload imbalance issue in 4D training: long document in CP, unbalanced document length distribution across micro-batch
    - Root cause: variations in per-token computation intensity result in workload imbalances
- Design a variable length input packing and adaptive outlier delay strategy

## Pros
- Illustrate the tradeoff of packing documents to reduce workload imbalance and model training loss
- Explain the hardware architecture's influence on workload sharding (CP).

## Cons
- Propose the parallelism hierarchies, but it does not describe the actual implementation order
- Larger batch size could be the reason of the increased loss (or the paper has not specify how the loss is compared. It should be the comparison between packing and not packing)
- Better CP sharding could interfere with the document packing output