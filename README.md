# Robotic Arm Contiuous Control

## About the Project
In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location.

* Observation space is 33 variables corresponding to position, linear and angular velocities and so.
Action space is 4 variables corresponding to Torque applied to two joints

* The goal of the agent is to maintain its position at the target location for as many time steps as possible.

* The environment is considered solved when the agent gets an average score of **+30 over 100 consecutive episodes**.

* The strategy learnt must get the agent am minimum average score of +13 over 100 consecutive episodes.

## Dependencies & Environment Setup
* install python 3.6
* Clone the DRLND Repository! and follow the README.md instructions to install PyTorch, the ML-Agents toolkit, and a few more Python packages required to complete the project.
* Download the ready-built Unity Environment:
* Linux
* Windows 64 3.Mac
* Place the file in the p1_navigation/ folder in the DRLND GitHub repository, and unzip (or decompress) the file

## About the code:
* Continuous_Control.ipynb contains the master code where the agent learn and the resulting models are saved.

* ddpg_agent.py contains the definition of the actor-critic architecture of the agent with its methods (act, step, learn), in addition to two utility classes (Ornstein-Uhlenbeck process noise generator & the replay buffer).

* model.py contains the actor-critic nn module architecture defining the number of layers, their dimensions, batch normalization and the activation used at the output layer.
