
# Overview  

This project is part of the Policy-Based Methods course in Udacity's Deep Reinforcement Learning Nanodegree. The goal of this project is to train a reinforcement learning agent in the Unity ML-Agents Reacher environment (a two linkage-robotic arm) to maintain its end effectory in the goal location for as many timesteps as possible. 

## Environment
The agent's state is fully observable. The observation/state size is 33 and the action size is 4, corresponding to four torque commands for the two joints. 

At each timestep, the agent receives a reward of +0.1 if the agent's end effector is in the goal location. We leverage 20 parallel agents to learn how to maximize expected cumulative reward. The aim is to train the agent to select the best action so that the agent is able to receive an average reward (over 100 episodes, and over all 20 agents) of at least +30. 

## Agent
The agent is an implementation of the Deep Determinstic Policy Gradient algorithm. Details will be discussed further in the included report.

# Installation

- To set up an Anaconda environment to run this code, you can follow the instructions included [here](https://github.com/udacity/deep-reinforcement-learning#dependencies). These instructions include:

  - Creating a new environment
  - Installing OpenAI gym
  - Cloning Udacity's deep reinforcement learning repository and installing dependencies
  - Creating and running the IPython kernel in the Jupyter notebook that provides the solution to this project. 
- The needed executable (Reacher.exe) for the environment is included in this repository and works for Windows 10 (64 bit).

# Usage
- The solution to this project is provided in the Navigation notebook (Continuous_Control.ipynb). Run each section of the notebook sequentially to train the agent. (You can skip Section 3, "Take Random Actions in the Environment," as this only displays random behavior of an untrained agent.)
- To view the details of the DDPQ implementation, see model.py and ddpg_agent.py. 
