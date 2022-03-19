# Reinforcement Learning Exercise in OpenAI Gym
This repository sharing my practice on Reinforcement Learning (RL) in the OpanAI Gym  http://gym.openai.com by different RL methods.

### Environments provided in OpenAI:
1. Atari
2. Box2D
3. Classic Control

### Logs:
2022-03-19 Uploaded ***Class Control - MountainCar-v0 added Epsilon-Greedy Policy.ipynb***

***Executive Summary:***

I added 2 sections in the last Class Control - MountainCar-v0 notebook. The Agent with ***Epsilon-Greedy Policy did not learn well in 100 epoch***, and then I revised the network remain with 4 layers but ***decrease trainable params to 8,835*** and ***increase number of epoch to 500***, set the learning procress stop when ***the mean of session rewards > -85*** (which is the performance of the second agent in section 5.3 last notebook. The ***learning process stop at epoch #274 (time spend: 1hr 48min)*** and the car reaches the flag on the right.

<img src='http://gym.openai.com/videos/2019-10-21--mqt8Qj1mwo/MountainCar-v0/poster.jpg' width='250px'/>

2022-03-17 Uploaded ***Class Control - MountainCar-v0.ipynb***

***Executive Summary:***

In this notebook, a car is on a one-dimensional track, positioned between two "mountains". ***The goal is to drive up the mountain reaches the flag on the right***. I try differnet methods to complete this goal, by comparing the retrained agent with more training steps (total 500k) and larger learning rate (1e-3), the car reaches the flag on the right with ***20% timesteps saving than the simple policy*** without any learning and ***32% timesteps saving than the agent with less training timesteps (total 200k) and smaller learning rate (1e-4)***.

----------------------------------------------------------------------------------------------------------
2022-03-14 Uploaded ***Atari - SpaceInvaders-v0.ipynb***

<img src='http://gym.openai.com/videos/2019-10-21--mqt8Qj1mwo/SpaceInvaders-v0/poster.jpg' width='250px'/>

***Executive Summary:***

I tried to ***build a deep learning model with Tensorflow for reinforcement learning*** and ***training a live reinforcement learning model using Keras-RL***. By comparing the agent's performance different between training for 100k timesteps and 1 million timesteps. The result show that ***the Agent's performance after training for 1 million timesteps perfrom 42.7% better in terms of average scores received***, and ***time spend more than 21 hours to train for 34,852,326 trainable params in 100k timesteps by CPU***.

----------------------------------------------------------------------------------------------------------

2022-03-13 Uploaded ***Atari - MsPacman-v0-3M_timesteps.ipynb***

<img src='http://gym.openai.com/videos/2019-10-21--mqt8Qj1mwo/MsPacman-v0/poster.jpg' width='250px'/>

***Executive Summary:***

I tried to ***compare the agaent's performance different between training for 1 million and 3 million timesteps*** by using exactly the same parameters except number of timesteps to train both agents. The result show that ***the Agent's performance after training for 3 million timesteps perfrom 55% better in terms of scores received***, but the ***time spending for training by CUP are 3 times more*** compare to the Agent's performance after training only for 1 million timesteps.  

Hope you enjoy it! Please share with me if you have even better solution or some other interesting environment for practicing RL purpose.
