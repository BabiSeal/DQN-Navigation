# DQN (Deep Q-Network) Agent for Unity Banana Navigation
Submission for Udacity Deep Reinforcement Learning NanoDegree

### Background

Train an agent to navigate around in a large square world and collect yellow bananas.  

[!Alt Text](https://video.udacity-data.com/topher/2018/June/5b1ab4b0_banana/banana.gif)

There is a reward of +1 to collect a yellow banana and a reward of-1 if you collect a blue banana. The goal is to collect as many yellow bananas as possible while avoiding the blue bananas.

 This environment has been kindly provided by Unity is provided by [Unity Machine Learning agents]([https://github.com/Unity-Technologies/ml-agents](https://github.com/Unity-Technologies/ml-agents)). 
#### State Space

The state space has 37 dimensions containing the agent's velocity along with ray-based perception of objects around the agent's forward direction.
#### Action Space

The agent has four discrete actions it can impact the environment by:
0. Move Forward
1. Move Backward 
2. Turn Left 
3. Turn Right

This is an episodic task where the agent has to learn how best to best selection actions.

#### When Solved

In order to solve this environment the agent must get an average of +13 over 100 consecutive episode

### Getting Started


#### Install Dependencies and needed files

The project was finally completed using the Udacity's workspace environment enabled with GPU support. The workspace environment uses the Unity ML-Agent v0.4 interface. 

We would strongly recommend using the ML-Agent v0.4 interface as attempts to coordinate the latest version of ML-Agents, grpcio, Pytorch modules with the latest version of Python installed, in Colab environments were not successful.
##### Dependencies
- Python 3
- Pytorch
- Unity ML-Agents v0.4
- Jupyter 
##### Installing the Environment

Again we would recommend using Udacity's provided provided workspace. If you wish to execute this locally, please download the appropriate image based on your operating system
- Linux: [download](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
- Max OSX: [download](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
- Windows (32-bit): [download](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
- Windows (64-bit): [download](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
- AWS: [download](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip)
### Instructions

#### Files
- `Navigation.ipynb` : The main Jupyter notebook to execute the training.
- `dqn_agent.py`: The Deep Q Network Agent that implements the learning algorithm as outlined in the paper [Human-level control through deep reinforcement learning](https://storage.googleapis.com/deepmind-media/dqn/DQNNaturePaper.pdf)
- `model.py` : The neural network that maps inputs to action probabilities
- `checkpoint.pth`:  The trained checkpoints. Load the checkpoints to avoid training the model from scratch. 

#### Training the Agent

Follow the exercises in `Navigation.ipynb` to train your agent using DQN 
