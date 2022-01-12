# Deep-RL-MountainCar-v0-Double-DQN


This project consist on using the Double Deep Q-Network (DDQN), a deep reinforcement learning method, on our envirement </br>"MountainCar-v0".

## MountainCar-v0
A car is on a one-dimensional track, positioned between two "mountains". The goal is to drive up the mountain on the right; however, the car's engine is not strong enough to scale the mountain in a single pass. Therefore, the only way to succeed is to drive back and forth to build up momentum


https://user-images.githubusercontent.com/56199509/147658904-81bcb85b-6d6e-4bb0-bf59-e0ac5d9b78ec.mp4

### Libreries

import numpy as np<br />
import gym<br />
import matplotlib.pyplot as plt<br />
import gc<br />
import random<br />
import time<br />

from collections import deque,namedtuple<br />
from IPython.display import clear_output<br />

from tensorflow.keras.models import Sequential, load_model<br />
from tensorflow.keras.layers import Dense<br />
from tensorflow.keras.initializers import he_normal<br />
from tensorflow.keras.optimizers import SGD<br />
from tensorflow.keras import models<br />

import torch<br />
import torch.nn as nn<br />
import torch.optim as optim<br />
import torch.nn.functional as F<br />
import copy<br />
## How it works
import libreries<br />
import the envirement<br />
### test with random actions



<p align="center">
<video  width="800" src="https://user-images.githubusercontent.com/56199509/147673060-5ec524ca-e5e6-4ffa-adb7-b61f87050b91.mp4" />
</p>
<br />

### test with DQN
#### create the Replay buffer<br />


<p align="center">
  <img width="800" src="https://user-images.githubusercontent.com/56199509/149232813-effc313b-c8b9-44ec-a4cc-7c2e60477877.PNG" />
</p>
<br />


#### create DQN class<br />

<p align="center">
  <img width="800" src="https://user-images.githubusercontent.com/56199509/149231328-121d0035-09c7-4bda-9d0c-82f708656dd9.PNG" />
</p>
<br />

#### create agent class<br />

<p align="center">
  <img width="800" src="https://user-images.githubusercontent.com/56199509/149231501-7f4840e9-f841-4e7d-8fe4-ed0f57db55f2.PNG" />
</p>
<br />

#### Training<br />

<p align="center">
  <img width="800" src="https://user-images.githubusercontent.com/56199509/149231804-c05f2c4a-ffed-4d60-a13a-a3afbb58655c.PNG" />
</p>
<br />

#### Training<br />

<p align="center">
  <img width="800" src="https://user-images.githubusercontent.com/56199509/149231629-2a943add-c665-4bcb-bf9d-7727db4aa642.PNG" />
</p>
<br />

<p align="center">
<video  width="800" src="https://user-images.githubusercontent.com/56199509/149233494-f7ed99f4-b90d-4d9d-ad09-abfe2628a465.mp4" />
</p>
<br />






### test with Double DQN

#### initialize hyper parameters<br />

<p align="center">
  <img width="800" src="https://user-images.githubusercontent.com/56199509/149232266-2c22a2f8-e51b-4cbb-b5a8-fba46286f402.PNG" />
</p>
<br />


#### train the model<br />

<p align="center">
  <img width="800" src="https://user-images.githubusercontent.com/56199509/149232351-193c1197-8256-4fb3-a171-c9ec4b550d93.PNG" />
</p>


#### Save the model and load it 


<p align="center">
  <img width="800" src="https://user-images.githubusercontent.com/56199509/147676391-fbbbc784-c94c-4840-8cea-c72f7d4bfcd4.png" />
</p>
<br />

#### Test the model
<p align="center">
<video  width="800" src="https://user-images.githubusercontent.com/56199509/147676212-8cde2f42-1f78-437d-a305-75e4fb9144da.mp4" />
</p>
<br />

