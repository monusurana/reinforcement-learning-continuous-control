[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/43851024-320ba930-9aff-11e8-8493-ee547c6af349.gif "Trained Agent"

# Project 2: Continuous Control

**NOTE:** I trained it on Udacity workspace and uploaded the model and notebook here. 

### Introduction

For this project, I worked on [Reacher](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#reacher) environment (Version 1)

![Trained Agent][image1]

#### Reward 
In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

#### State Space
The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. 

#### Action Space 
Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

#### Goal 

The task is episodic, and in order to solve the environment,  your agent must get an average score of +30 over 100 consecutive episodes.

### Getting Started

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:

    - **_Version 1: One (1) Agent_**
        - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip)
        - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)
        - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86.zip)
        - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86_64.zip)

    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

### Train Agent

Execute `Continuous_Control.ipynb` to train your own agent! It is based on DDPG([Paper](https://arxiv.org/pdf/1509.02971.pdf)). 

The entire notebook can be executed by pressing play icon

![Jupyter Image](resources/ExecuteEntireNotebook.png)

The trained agents would automatically get saved in ```models/``` folder for each of the algorithms 

### Folder Structure 

- ```agents``` contains the code for all the types of agents 
- ```buffers``` contains the code for replay buffer which all the algorithms use 
- ```models``` contains the saved models generates by the code 
- ```networks``` contains the code for neural networks being used by all the algorithms 
- ```resources``` contains all the resources related with project
