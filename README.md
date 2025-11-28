# Q-Learning-Based Trading Environment — Developed a custom trading environment and trained a tabular Q-learning agent to maximize profit on historical market data :

In this project, we use historical price data for Web Mellat stock from '1397-01-01' to '1404-04-20'. The dataset is split into two subsets: 80% for training and 20% for testing.

We apply the following tabular Q-learning algorithm:

<div justify-content: center; >
<img src="https://leimao.github.io/images/blog/2019-03-14-RL-On-Policy-VS-Off-Policy/q-learning.png" alt="Girl in a jacket" width="800" height="900">
</div>


We define the state space as a three-dimensional vector:

$$\mathcal{S} = \left[ (r, rsi , v) \mid r \in \text{return binned} , rsi \in \text{RSI binned} , v \in \text{volume binned} \right]$$

The reward at time \(t\) is defined as:

$$r_t = \text{position}_t \times \text{return}_t - \text{trading cost}$$

Additional implementation details and experiments are provided in the accompanying Jupyter notebook.﻿

  


