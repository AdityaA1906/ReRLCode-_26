# MountainCarContinuous-v0 with DDPG

## Overview
This repository contains an implementation of the Deep Deterministic Policy Gradients (DDPG) algorithm, as described in the paper **"Continuous control with deep reinforcement learning" by Lillicrap et al**, evaluated on the MountainCarContinuous-v0 environment from the Gymnasium library.

DDPG is an actor-critic, model-free algorithm tailored to continuous action domains. Building on the deterministic policy gradient (DPG) framework, DDPG adapts techniques from Deep Q-Network (DQN) like experience replay and target networks to stabilize training and handle high-dimensional, continuous action spaces. This implementation uses PyTorch's **LayerNorm** instead of batch normalization, as it is invariant to batch size and allows for a cleaner implementation of the target network parameter updates.

## Setup

### Install Dependencies
```
pip install -r requirements.txt
```

### Run Training
```
python main.py --env 'MountainCarContinuous-v0'
```

## Results
![Running Average](metrics/MountainCarContinuous-v0_running_avg.png)

![MountainCar](environments/MountainCarContinuous-v0.gif)
