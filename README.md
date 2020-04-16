# DRL-Projects
This is repo is based on Udacity's Nanodegree on [Deep Reinforcement Learning](https://www.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893) 

# Deep Q Network: Navigation
This project repository contains the code and references to implement a DQN for solving a navigation problem in Banana Simulator.

# About DQN
Q learning + Neural Network  = Deep Q Network 
In DQN we use Neural Network to approximate Q table.

# Environment details
The environment is based on [Unity ML-agents](https://github.com/Unity-Technologies/ml-agents).
Note: The project environment provided by Udacity is similar to, but not identical to the Banana Collector environment on the Unity ML-Agents GitHub page.

The agent is trained using Pytorch to navigate through the environment and  collect yellow bananas.  For every yellow banana the agent receives a reward of +1 and for every blue banana it receives a rewards of -1.  The agent is trained to avoid the blue banana as much as possible.

The state space has 37 dimensions and the action space has 4 actions each for  moving the four directions.

The task is episodic and the episode ends after achieving a reward of +13 over 100 consecutive episodes.

# Resources
A cheat sheet is provided by Udacity for studing reinforcement learning.
This repo has 3 code files – model.py, dqn_agent.py and Navigation.ipynb

# Getting started
# Installation requirements
The repository contains material related to Udacity's Deep Reinforcement Learning Nanodegree program.

Download the environment from one of the links below. You need only select the environment that matches your operating system:
Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)

Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)

Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)

Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)

Place the file in the DRLND GitHub repository, in the p1_navigation/ folder, and unzip (or decompress) the file.
# Instructions
Follow the instructions in Navigation.ipynb to get started with training your own agent!

# Obtained Output
![score](https://github.com/vickyskarthik/DRL-Projects/blob/master/output/score_vs_episodes_dqn.png)

Environment solved in 430 episodes 
Average Score: 13.00
Total Training time = 11.4 minutes

![score](https://github.com/vickyskarthik/DRL-Projects/blob/master/output/score_vs_episodes_dqn2.png)


# Future Works
So far the agent is trained only using DQN which can also be implemented using Double DQN and Pritorized Experience Replay and Dueling DQN to increase their performance.   
Also in this attempt the agent interacted with the environment but the agent can be trained using raw pixels from the environment as input.

# Reference
[1] Juliani, A., Berges, V., Vckay, E., Gao, Y., Henry, H., Mattar, M., Lange, D. (2018). Unity: A General Platform for Intelligent Agents. [arXiv preprint arXiv:1809.02627.] (https://github.com/Unity-Technologies/ml-agents)

[2] R. S. Sutton and A. G. Barto, Introduction to Reinforcement Learning, 2nd ed. Cambridge, MA, USA: MIT Press, 2017

