[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135623-e770e354-7d12-11e8-998d-29fc74429ca2.gif "Trained Agent"
[image2]: https://user-images.githubusercontent.com/10624937/42135622-e55fb586-7d12-11e8-8a54-3c31da15a90a.gif "Soccer"

# Deep RL Collaboration and Competition Tennis
Udacity Deep Reinforcement Learning Nanodegree, third project "Collaboration and Competition".

# Project 3: Collaboration and Competition.
The learning algorithm to solve the task was a DDPG controlling both players and trained via self-play and shared replay buffer, for details see the report.

### Environment

In this project the [Tennis](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#tennis) environment is solved. 
The goal of both agents playing against each other is to keep the ball in play.

![Trained Agent][image1]

### Rewards 

In this environment, two agents control rackets to bounce a ball over a net. If an agent hits the ball over the net, it receives a reward of +0.1.  If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01.

The task is episodic, and in order to solve the environment, your agents must get an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents).

### States and Actions

The observation space consists of 24 dimensions corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation.  Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping. 


### Files in this Repository
                    
    .
    ├── checkpoint_actor_64x64.pth          # stored weights for trained actor network (2 hidden 128 unit layers)
    ├── checkpoint_actor.pth                  # latest stored weights for trained actor network
    ├── checkpoint_critic_64x64.pth         # stored weights for trained critic network (2 hidden 128 unit layers)
    ├── checkpoint_critic.pth                 # latest stored weights for trained critic network
    ├── Tennis.ipynb                          # main code for training and testing the agent
    ├── ddpg_agent.py                         # agent to interact and learn from environment
    ├── model.py                              # neural network model (in Pytorch)
    ├── Report.pdf                            # report of the implementation and details of the learning algorithm
    └── README.md


### Python Packages
 
 - collections
 - copy
 - matplotlib
 - numpy
 - random
 - torch
 - unityagents
 
 **Note:** The Unity environment did not work on Mac OS for Python version 3.7 and higher. Python version 3.6 worked well.


### Downloading the Environment

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86_64.zip)

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux_NoVis.zip) to obtain the "headless" version of the environment.  You will **not** be able to watch the agent without enabling a virtual screen, but you will be able to train the agent.  (_To watch the agent, you should follow the instructions to [enable a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md), and then download the environment for the **Linux** operating system above._)


### Instructions

Follow the instructions in `Tennis.ipynb` to get started with training your own agent!  
