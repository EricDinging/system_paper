# [FATE-LLM: A Industrial Grade Federated Learning Framework for Large Language Models](https://arxiv.org/pdf/2310.10049)
## Problem
1. Training LLM consumes vast computing resources
2. Training LLM requires a large amount of data
## Backgrounds

## Challenges

## Observations
Use federated learning to solve these problems
## Ideas
Build upon 

## Contribution

## Methods
Build upon FATE

## Results

1. Enables federated learning for
both homogeneous and heterogeneous large language models
2. Promotes efficient training of FedLLM
through parameter-efficient fine-tuning methods, such as
LoRA
3. Protects the intellectual property of LLMs
4. Protects data privacy during training and inference through privacy-preserving mechanisms

Specifically, Fate-llm has four components
1. Communication efficient hub, includes methods such as PETuning
2. Model hub
3. Trainer hub, including various training methods FedHomoLLM, FedHeteroLLM, FedCoLLM, and
FedOST
4. Privacy hub

### FedHomoLLM
Clients have LLMs with the same architecture leverage PEFT to train their LLMs

### FedHeteroLLM
Clients have LLMs with different architecture leverage knowledge distillation and PEFT to train their LLMs.

### FedCoLLM
Not only clients but also the server owns LLMs. They leverage PEFT and knowledge
distillation to fine-tune their LLMs.

### FedOST
Clients transfer their knowledge to the LLM hosted by the server through offsite-tuning in a federated way.

## Application

## Limitation
- Small clients (2 clients) and LAN network environment in experiments
- Claim a scale of 30 clients maximum
- Inferior in performance than centralized counterpart, slight improvement over client trained models

## Related concepts
1. Knowledge distillation https://pytorch.org/tutorials/beginner/knowledge_distillation_tutorial.html
2. Adapter/prompt vs. finetuining
3. PEFT
4. LoRa