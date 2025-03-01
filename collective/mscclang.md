# [MSCCLang: Microsoft Collective Communication Language](https://parsa.epfl.ch/course-info/cs723/papers/MSCCLang.pdf)

## Summary
MSCCLang focuses on software stack to program and optimize collective communication algorithms within existing hardware, achieving faster collectives user NCCL

The key design behind MSCCLang is the chunk-oriented DSL, enabling parallelization and pipelining.

## Limitation
Limits the number of connections on one channel

The speedup over NCCL is limited over input sizes.


## Questions
What are inter-instruction dependencies