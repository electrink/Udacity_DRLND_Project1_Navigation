# Udacity_DRLND_Project1_Navigation
In this repository, I provide source codes for implementing a double deep Q-network (DQN) to solve the navigation (banana collection) problem in the Unity ML-Agents environment. This is the first project in Udacity's Deep Reinforcement Learning Nano Degree (DRLND) program.

## Environment
The environment is provided by DRLND’s course website. For this project, I am asked to train an agent to navigate (and collect bananas!) in a large, square world. A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of my agent is to collect as many yellow bananas as possible while avoiding blue bananas. 

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

- 0 Move forward
- 1	Move backward
- 2	Turn left
- 3	Turn right

The task is episodic, and in order to solve the environment, my agent must get an average score of +13 over 100 consecutive episodes. To make the task a little bit more chanllening, I set the bar at +15 and saved the model weights of teh successful agent aginst this criterion.

## Getting Started
### Prerequisites
The following list of required dependencies are based on a Win7 64-bit system.

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
