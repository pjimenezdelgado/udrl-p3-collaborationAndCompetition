# Udacity Deep Reinforcement Learning - Project 3 - Collaboration and Competition
---------------------------------------------------------------------------------

This is the report for Project 3 - Collaboration and Competition from the Deep Reinforcement Learning Nanodegree of Udacity. 

## Project details

This is the report for Project 3 - Collaboration and Competition from the Deep Reinforcement Learning Nanodegree of Udacity. The task is to train two agents to control rackets to bounce a ball over a net. If an agent hits the ball over the net, it receives a reward of +0.1. If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01. Thus, the goal of each agent is to keep the ball in play. The task is continuous, although the episodes end after a certain time or when an agent fails. 

The observation space consists of 8 variables corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation. Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping. 

In order to solve the environment, the agents must get an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents). 

## Getting Started

The top level of the project has been developed as a Jupyter notebook (`Cennis.ipynb`) in Python 3, thus make sure that you have a running Python and Jupyter working installation.

The world is provided as an Unity environment titled "Tennis", and is external to the project itself. To install the environment you will need a distribution of the ml-agents package from Unity. The location of the repo could potentially change, but at the moment of writing the link to the environment is:

`https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#tennis`

Please follow the installation instructions there, as these may change; in our case we used the environment supplied by Udacity. 

The agent is provided in `dpqg_agent.py`, and the underlying neural network models in `model.py` (both these files were obtained from Udacity Qnetwork project and tweaked). For these to run one needs to install Pytorch; other packages that need to be imported directly are numpy, and matplotlib. To install them, please run

`pip install numpy matplotlib pytorch`

In addition all these packkages will have dependencies themselves, which need to be satisfied before proceeding. A complete list of all the dependencies can be found in `requiriments.txt`, and istalled using

`pip requirements.txt`

## Instructions

The notebook is pretty much self-contained. It contains only three cells. 

- Run the first one one to set up the angents and the environment itself.
- The second one provides the code for the training itself, run this if you want to train the agents.
- The third one is optional, provides some information about the environment and basic usage interface of the agents and its interactions with the environment, as well as an example of how to use them. This can be used to evaluate the trained or untrained agents. Watch them play one episode, it is fun!
