# Deep-RL-MountainCar-v0-Double-DQN


This project consist on using the Double Deep Q-Network (DDQN), a deep reinforcement learning method, on our envirment "MountainCar-v0".

## MountainCar-v0
A car is on a one-dimensional track, positioned between two "mountains". The goal is to drive up the mountain on the right; however, the car's engine is not strong enough to scale the mountain in a single pass. Therefore, the only way to succeed is to drive back and forth to build up momentum


https://user-images.githubusercontent.com/56199509/147658904-81bcb85b-6d6e-4bb0-bf59-e0ac5d9b78ec.mp4

### Libreries

import numpy as np
import gym
import matplotlib.pyplot as plt
import gc
import random
import time

from collections import deque
from IPython.display import clear_output

from tensorflow.keras.models import Sequential, load_model
from tensorflow.keras.layers import Dense
from tensorflow.keras.initializers import he_normal
from tensorflow.keras.optimizers import Adam , SGD

## How it works
import libreries
import the envirement
### test with random actions
### test with DDQN
train the model
save the model 
load it then render the envirement
