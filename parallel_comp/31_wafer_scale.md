# Switch-Less Dragonfly on Wafers: A Scalable Interconnection Architecture based on Wafer-Scale Integration

## Please write a summary of the paper [from 3 to 6 sentences].
The paper proposes an interesting network interconneciton design based on Dragonfly topology that removes costly switches and uses wafer-scale systems for interconnection. The paper proposes routing mechanism and virtual channels assignment for dead-lock free routing. The evaluation shows that the topology has high local injection bandwidth and comparable global bandwidth to other topologies.

## Please highlight the strengths of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some strengths].
- The switch-less architecture only requires one additional virtual channel compared to traditional Dragonfly.
- The work shows layout design for ultra-high density of wafer scale integration.
- The work shows that the topology could have higher local injection bandwidth and comparable global injection bandwidth compared to other topologies.

## Please highlight the weaknesses of the paper [from 3 to 6 sentences, "NA" is not an acceptable response, every work has some weaknesses].
- There is no discussion of fault tolerance.
- The evaluation only focuses on injection metrics and power consumption.
- The 2D mesh has limited bisection bandwidth, limiting global bisection bandwidth.

## Please provide a question for in-class discussion.
How could 2x and 4x on-wafer bandwidth in the evaluation be achieved?

## Please provide a question for in-class discussion.
Will boundary chiplet experience be overloaded due to inter-wafer communication?
