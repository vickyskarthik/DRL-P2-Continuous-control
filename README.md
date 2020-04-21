# DRL-Projects
This is repo is based on Udacity's Nanodegree on [Deep Reinforcement Learning](https://www.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893) 

<<<<<<< HEAD
# Continuous Navigation
This project repository contains the code and references to implement a DQN for solving a navigation problem in Banana Simulator.
=======
# The Environment
For this project, you will work with the Reacher environment.
>>>>>>> f904e8cb569325b5033774e08a556c6fba1e55a9

In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

# Distributed Training
For this project, we will provide you with two separate versions of the Unity environment:

The first version contains a single agent.
The second version contains 20 identical agents, each with its own copy of the environment.
The second version is useful for algorithms like PPO, A3C, and D4PG that use multiple (non-interacting, parallel) copies of the same agent to distribute the task of gathering experience.

# Solving the Environment
Note that your project submission need only solve one of the two versions of the environment.

# Option 1: Solve the First Version
The task is episodic, and in order to solve the environment, your agent must get an average score of +30 over 100 consecutive episodes.

# Option 2: Solve the Second Version
The barrier for solving the second version of the environment is slightly different, to take into account the presence of many agents. In particular, your agents must get an average score of +30 (over 100 consecutive episodes, and over all agents). Specifically,

After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 20 (potentially different) scores. We then take the average of these 20 scores.
This yields an average score for each episode (where the average is over all 20 agents).
As an example, consider the plot below, where we have plotted the average score (over all 20 agents) obtained with each episode.

# Criteria
The environment is considered solved, when the average (over 100 episodes) of those average scores is at least +30. In the case of the plot above, the environment was solved at episode 63, since the average of the average scores from episodes 64 to 163 (inclusive) was greater than +30.

# Solution
The algorithm used to solve this problem is [Deep Deterministic Policy Gradient(DDPG).](https://spinningup.openai.com/en/latest/algorithms/ddpg.html)

# Why choose Policy Based Method?
1. Simplicity
2. Well suited for continuous action space
3. stochastic policy

# Future Works
So far the agent is trained only using DQN which can also be implemented using Double DQN and Pritorized Experience Replay and Dueling DQN to increase their performance.   
Also in this attempt the agent interacted with the environment but the agent can be trained using raw pixels from the environment as input.

# Reference
[1] John Schulman, Filip Wolski, Prafulla Dhariwal, Alec Radford, Oleg Klimov, [Proximal Policy Optimization Algorithms ](https://arxiv.org/abs/1707.06347)

[2] Juliani, A., Berges, V., Vckay, E., Gao, Y., Henry, H., Mattar, M., Lange, D. (2018). Unity: A General Platform for Intelligent Agents. [arXiv preprint arXiv:1809.02627.] (https://github.com/Unity-Technologies/ml-agents)

[3] R. S. Sutton and A. G. Barto, Introduction to Reinforcement Learning, 2nd ed. Cambridge, MA, USA: MIT Press, 2017

[4] [Deterministic Policy Gradient Algorithms](http://proceedings.mlr.press/v32/silver14.pdf), Silver et al. 2014

[5][Continuous Control With Deep Reinforcement Learning](https://arxiv.org/abs/1509.02971), Lillicrap et al. 2016

