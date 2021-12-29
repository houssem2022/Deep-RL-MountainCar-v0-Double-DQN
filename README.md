# Deep-RL-MountainCar-v0-Double-DQN


This project consist on using the Double Deep Q-Network (DDQN), a deep reinforcement learning method, on our envirment "MountainCar-v0".

## MountainCar-v0
A car is on a one-dimensional track, positioned between two "mountains". The goal is to drive up the mountain on the right; however, the car's engine is not strong enough to scale the mountain in a single pass. Therefore, the only way to succeed is to drive back and forth to build up momentum


https://user-images.githubusercontent.com/56199509/147658904-81bcb85b-6d6e-4bb0-bf59-e0ac5d9b78ec.mp4

### Libreries

import numpy as np /n
import gym /n
import matplotlib.pyplot as plt/n
import gc\n
import random\n
import time\n

from collections import deque\n
from IPython.display import clear_output\n

from tensorflow.keras.models import Sequential, load_model\n
from tensorflow.keras.layers import Dense\n
from tensorflow.keras.initializers import he_normal\n
from tensorflow.keras.optimizers import Adam , SGD\n

## How it works
import libreries\n
import the envirement\n
### test with random actions
![image](https://user-images.githubusercontent.com/56199509/147672490-8adbad68-0caf-46a5-9e1e-255c8500242b.png)


https://user-images.githubusercontent.com/56199509/147673060-5ec524ca-e5e6-4ffa-adb7-b61f87050b91.mp4



### test with DDQN
initialize hyper parameters\n

![image](https://user-images.githubusercontent.com/56199509/147672586-16c2496d-b522-4955-a4fc-c5db1eb2399d.png)\n

train the model\n
![image](https://user-images.githubusercontent.com/56199509/147673600-9fbe0d92-55f1-4a48-b915-6456cb2cc02b.png)\n

save the model \n
load it then render the envirement\n
