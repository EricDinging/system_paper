# CAPE: A Content-Addressable Processing Engine

## Please write a summary of the paper [from 3 to 6 sentences].
The research proposes a CMOS-based content addressable memory arrays and a microarchitecture that could perform parallel data operation on top of the memory arrays. This PIM architecture can support bit-serial arithmetic and logic operations. Experiments show that CAPE achieves an average speedup of 14 over an area-equivalent out-of-order processor core.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
1. The whole architecture achieves order-of-magnitude speedup over conventional solution.
2. The approach is integrated with a traditional ISA, without the need for programming language or compiler change.
3. The researchers conducted holistic modelling to study the architecture performance, and focused on important metrics such as energy for CAM,

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
1. CAPE does not have a cache, which could result in poor performance when the application has high temporal locality.
2. The paper does not give an example when CAPE is superior than out-of-order engine.
3. The solution is limited to synthesis result.

## Please provide a question for in-class discussion.
Is it possible to perform multiple reads or writes at the same time, each with different commands?

## Please provide a question for in-class discussion.
CAPE could mask the unused CSB columns if the vector size is small. What is the strategy if the vector size exceeds the width of CAPE?


