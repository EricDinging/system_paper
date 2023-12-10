# [DataPrism: Exposing Disconnect between Data and Systems](https://dl.acm.org/doi/pdf/10.1145/3514221.3517864)
## Problem
- what properties of a dataset caused the failure of system
## Challenges

## Observations
- Two causes
    - Incorrect data
    - Disconnection on the assumptions about the data and system design
- Results
    - Decline in accuracy
    - Unfairness in model prediction
    - Excessive processing time
    - System crash
## Ideas
- Come up with a hypothesis. eg: Identify outliers
- Verify the hypothesis.
    - Data profiler
    - Oracle-guided root cause identification
## Methods
- An intervention mechanism that alters the profile of the dataset
- A mechanism that speeds up analysis
- Requires:
    - Well-known set of relevant profiles
    - Domain expert predicate

## Results

## Application
- Agnostic to systems

## Limitation
- Cannot prevent failure from happening
## Questions