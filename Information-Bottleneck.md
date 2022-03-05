Information-Bottleneck methodes about finding a representation which is necessary about the task constrained on little mutual information between input and ouput representation.


Note:
There is a naunce between the goal of Information-Bottleneck and applying the constraint of information neccessary for the task on Minimum Description Length(MDL). It is due to the fact that
in Information-Bottleneck methodes, the representation could have other sources information ohter than the input data, the stochastic representation and meet up the goal in information bottelneck. In MDL, however,  it seems that you should only have a deterministic representation to have minimum length on the ground that each stochsstic represntation introduce redundant bits of information



Question

- So why we need stochastic representations

One possible solution to the above question is that task needs some information other than the one in input data ! unless in terms of MDL, adding any new source of information other than input data increase description length.