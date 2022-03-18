![[Representation Learning and MDP.svg]]



On the ground that we don't know what information is usefull for a down stream task, we can not directly set Objective Function in RL.    


One approach to handle it in the contex of MDP is to Learn Reward Function or Objective Function. In the contex of RL with MDP view of mind, learning the model of the environment is not the matter fact. Instead the Reward function lead us to the Optimal policy (Stochastic mapping or representation) in terms of keeping usefull information for a downstream task. Keeping this scenario in the mind, our attention come to the MDP with uncertain reward function.


MDP with uncertain reward function

Inversive Reinforcement Learning:

In inversive Reinforcemnt Learning we don't know reward as well as transition probabilities we only know samples of the optimal trajectories( state - action) from a state to the best state of an expert and we need to make infference what is the reward optimized the trajectorize samples of expert. In other word, we need to know what reward function dose expert use in order to generate optimal these path for the reward function. 


In constrasitve Learning, the ouput samples of agumnetation can be seen as samples of optimal trajectories by the expert. Actually these samples tell which infomation is usefull which are not. This statement needs to be more clearly demystified.