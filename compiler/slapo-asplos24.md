# Slapo: A Schedule Language for Progressive Optimization of Large Deep Learning Model Training


## Motivation
1. Optimization is not general to all GPU models
2. Ease of tuning.
3. Programmability. The compilier requires static graph, and other constraints
4. Debuggability: fattened execution graph vs hierarchical implementation.

## Design
1. Decouple model execution from its definition
2. Auto-tuning on the defined optimization space based on a separate schedule
3. Progressive optimization
4. Structure-preserving scheduling.