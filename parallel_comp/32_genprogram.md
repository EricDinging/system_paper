# Learning Generalizable Program and Architecture Representations for Performance Modeling

## Please write a summary of the paper [from 3 to 6 sentences].
This paper presents PerfVec, a ML-based performance modeling model. It uses deep learning model to extract high-level representation of the program and microarchitecture for downstream performance prediction. This approach is highly generalizable.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
- PerfVec autonomously disentangles performance factors from program and microarchitecture, enabling predictions for unseen combinations.
- The approach is generalizable to new programs.
- The representation reuse technique saves training time by orders of magnitude.

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
- The work can only support sequential program modelling.
- The method requires detailed instruction traces.
- The prediction may not be accurate for under-represented programs or hardware.

## Please provide a question for in-class discussion.
How do you tell the execution time if the program execution is data-dependent without some kind of compilation or pre-execution?

## Please provide a question for in-class discussion.
Is it feasible to conduct reinforcement learning based on real execution results?


