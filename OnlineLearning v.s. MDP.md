In online learning, by and large, we don't have any assumption on distrbution of observations


In supervised Learning view in mind, in online learning we don't have test and train datasets and so there is no concepts of generalization error. Instead, we have the concept of regret. Mathmatically speacking, in online learning, we deal with a hypothesis set and we look for the best hypothesis labeling the observations. 

$$Regret = \sum_{t=1}^{N} L(\tilde{y}_t, y_t) - \min_{y'_t} \sum_{t=1}^{N} L(y^{'}_t,y_t) $$
Considering the fact that there is a hypothesis from which the true labels for observations come, we need to select this hypothesis for labeling $x_t$, observation in  $t$th  step. Also in bounding there is no assumption on distribution of input data. 

Also, we have adverserial and the worst case assumptionin which there may be no fixed hypothesis for labeling data. In this case, we have two situation



Minmax problem in estimation, unsupervised learning, can be seen as a probablistic view of online learing in which we have assumption on distribution of data however again we can treat the probablistic family as a hypothesis set in the superivised learning view. 

$$ \sum_{t=1}^{N} L(\theta_t,\theta^*)$$

However, here from scratch we know that the best anwser, parmeter, is fixed n all steps, there is no adverserial with this concept in mind, and aslo $L$ is an expectation. However, we have the worst case senario in the same way as online learning 
**
The main difference  between MDP and common online learning is the assumption of distribution on observations.
** 

Although Our MDP framework for estimation is similar to online learning,  we have the assumption on the distribution and also we don't have adverserial assuption which is usual in the contex of online learnig. 

However, intiutinvely, each MDP problem can be converted to online learning on the ground that we can see the choise of policy in each steps as the choise of a hypothesis in hypothesis set and make action from that policy can be seen as labeling the observation using the choosed hypothesis. The regret can be seen as a distance between choosed policy and the best policy or the best hypothesis and choosed hypothesis or best action and choosed action or best label and choosed label.

However again we have different situations

The policy is stationary over steps == fixed hypothesis
The policy is not stationary == adverserial assuption changing hypothesis

MDP also is general in terms of the fact that the action does't have to be made after each observation 