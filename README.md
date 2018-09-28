# Udacity_DRLND_Project1_Navigation
In this repository, I provide source codes for implementing a double deep Q-network (DQN) to solve the navigation (banana collection) problem in the Unity ML-Agents environment. This is the first project in Udacity's Deep Reinforcement Learning Nano Degree (DRLND) program.

## Environment
The environment is provided by DRLND’s course website. For this project, I am asked to train an agent to navigate (and collect bananas!) in a large, square world. A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of my agent is to collect as many yellow bananas as possible while avoiding blue bananas. 

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

- 0 Move forward
- 1	Move backward
- 2	Turn left
- 3	Turn right

The task is episodic, and in order to solve the environment, my agent must get an average score of +13 over 100 consecutive episodes. To make the task a little bit more chanllening, I set the bar at +15 and saved the model weights of the successful agent based on this criterion.

## Getting Started
### Prerequisites
- tensorflow==1.7.1
- Pillow>=4.2.1
- matplotlib
- numpy>=1.11.0
- jupyter
- pytest>=3.2.2
- docopt
- pyyaml
- protobuf==3.5.2
- grpcio==1.11.0
- torch==0.4.0
- pandas
- scipy
- ipykernel
- pickle
- collections
- unityagents

Note that to work properly in the Windows 7 64-bit environment, one has to mannualy place the following three folders - *unityagents*, *communicator_objects*, and *Banana_Windows_x86_64* - at the root of this working directory. This may or may not be the case for other operating systems.  

## Instructions
### Training
Open *P1_Navigation_Jing Zhao.ipynb* to start training an AI agent. This script interacts with the Unity ML-Agents environment to gain experience which is defined by visiting a new state and receiving a reward from the previous action. In addition, the script also uses the double DQN-based learning algorithm implemented in *dqn_agent_double.py* and *model.py* to improve the agent's performance over time.    

### Viewing the Result
After training is done, one can view the agent's performance across total episodes in *P1_Navigation_Jing Zhao.ipynb*. This result is stored in the *zipScore.pickle* file. The 100-point moving average of the score is also provided to check at what episode the environment is solved. One can also watch a smart agent to play the game. The *checkpoint_doubleQ_SOLVED-689.pth* recorded the model weights when the agent reached an average score of +15 over 100 consecutive episodes. Additionally, weights at 500, 1000, 1500, and 2000 episodes are also saved for viewing purpose.

## Author
Jing Zhao. Implementation of the double DQN network is inspired by the [Deep Q-Network (DQN)](https://github.com/udacity/deep-reinforcement-learning/tree/master/dqn) project in the DRLND program.
