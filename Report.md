# Continuous Control Reacher

##  Models

The actor model uses 3 Linear layers with 600 nodes apiece. The critic model uses 4 Linear layers with varying nodes each (600, 500, 400).

## Learning parameters

BUFFER_SIZE = int(2e5)  # replay buffer size

BATCH_SIZE = 128        # minibatch size

GAMMA = 0.99            # discount factor

TAU = 1e-3              # for soft update of target parameters

LR_ACTOR = 1e-4         # learning rate of the actor 

LR_CRITIC = 1e-4        # learning rate of the critic

WEIGHT_DECAY = 0.0000   # L2 weight decay

Learns from 3 samples at each step

For noise: mu=0, theta=0.8, sigma=0.1

## The results

The training reached an average of 30 on episode 56 and maintained that until episode 101.


## The future
I would definitely work to try make the algorithm work at a higher noise level. I would also potentially implement prioritized experience samples.
