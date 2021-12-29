# Deep-RL-MountainCar-v0-Double-DQN


This project consist on using the Double Deep Q-Network (DDQN), a deep reinforcement learning method, on our envirment "MountainCar-v0".

## MountainCar-v0
A car is on a one-dimensional track, positioned between two "mountains". The goal is to drive up the mountain on the right; however, the car's engine is not strong enough to scale the mountain in a single pass. Therefore, the only way to succeed is to drive back and forth to build up momentum


https://user-images.githubusercontent.com/56199509/147658904-81bcb85b-6d6e-4bb0-bf59-e0ac5d9b78ec.mp4

### Libreries

import numpy as np <br />
import gym <br />
import matplotlib.pyplot as plt<br />
import gc<br />
import random<br />
import time<br />

from collections import deque<br />
from IPython.display import clear_output<br />

from tensorflow.keras.models import Sequential, load_model<br />
from tensorflow.keras.layers import Dense<br />
from tensorflow.keras.initializers import he_normal<br />
from tensorflow.keras.optimizers import Adam , SGD<br />

## How it works
import libreries<br />
import the envirement<br />
### test with random actions

<p align="center">
  <img width="800" src="https://user-images.githubusercontent.com/56199509/147672490-8adbad68-0caf-46a5-9e1e-255c8500242b.png" />
</p>


<br />

<p align="center">
<video  width="800" src="https://user-images.githubusercontent.com/56199509/147673060-5ec524ca-e5e6-4ffa-adb7-b61f87050b91.mp4" />
</p>
<br />



### test with DDQN
#### initialize hyper parameters<br />

<p align="center">
  <img width="800" src="https://user-images.githubusercontent.com/56199509/147672586-16c2496d-b522-4955-a4fc-c5db1eb2399d.png" />
</p>
<br />

#### train the model<br />

<p align="center">
  <img width="800" src="https://user-images.githubusercontent.com/56199509/147673600-9fbe0d92-55f1-4a48-b915-6456cb2cc02b.png" />
</p>
<br />
#### save the model and load it <br />


<p align="center">
  <img width="800" src="https://user-images.githubusercontent.com/56199509/147676391-fbbbc784-c94c-4840-8cea-c72f7d4bfcd4.png" />
</p>
<br />

#### Test the model
<p align="center">
<video  width="800" src="https://user-images.githubusercontent.com/56199509/147676212-8cde2f42-1f78-437d-a305-75e4fb9144da.mp4" />
</p>
<br />

