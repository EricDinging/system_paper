# Single-Source Regular Path Querying in Terms of Linear Algebra

## Please write a summary of the paper [from 3 to 6 sentences].
The paper proposes a new algorithm for evaluating two-way regular path queries (2-RPQs) on edge-labelled graphs. This approach utilizes high-performance sparse linear algebra libraries to improve query performance. 2-RPQs allow for the use of regular languages over both forward and inverted edges, making them a powerful tool in graph analysis. The algorithm demonstrates significant speedup compared to existing methods when tested on real-world data, such as Wikidata.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
- The algorithm can efficiently handle large-scale graph data through using sparse linear algebra libraries
- The method is tested on Wikidata, showing its practicality.
- The evaluation is thorough, including the distribution of time spent during execution.

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
- The method may not generalize well to dynamic graphs.
- The paper does not show enough results about the scalability to bigger graphs.
- The paper does not discuss the scalability of this approach to mulitple quries (throughput).

## Please provide a question for in-class discussion.
- Would this approach still be efficient for dynamic graphs where edges are frequently added or removed?

## Please provide a question for in-class discussion.
- Could this method be extended to handle more complex graph queries?
