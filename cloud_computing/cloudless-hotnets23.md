# [Simplifying Cloud Management with Cloudless Computing](link)
## Problem
- Cloud infrastructure management is crucial
- Cloud automation frameworks, following Infrastructure-as-Code paradigm
    - Lack a principled design, leaky performance
    - Mapping from the IaC-level code constructs to the cloud-level APIs is quite involved
## Challenges
- Developing IaC infrastructure
- Validating IaC infrastructure
- Deploying IaC infrastructure
- Updating IaC infrastructure
- Diagnosing IaC infrastructure
- Policing IaC infrastructure

## Backgrounds

## Observations

## Ideas
- Cloudless computing
- Automated IaC synthesis
    - LLM frequently generate invalid IaC code, introduce security vulnerabilities
    - Decompose the infrastructure into its component elements
- Porting non-IaC infrastructures to IaC
- Validation, richer and easier symantics
- Deploying IaC, acceleration in updates
- Updating IaC
    - Concurrent updates and mutual exclusion, granular locking, a lock manager backed by an IaC database that reflects the ideal state of the cloud infrastructure
    - Rollback
- Diagnosing IaC infrastructure
- Policing enforcement with a controller
## Contribution

## Methods

## Results

## Application

## Limitation

## Questions