## Abstract

Training with Reinforcement Learning tipically requires a reward function that is used to guide the agent towards achieving its objective. However, designing smooth and well-behaved rewards is non-trivial and requires significant human engineering efforts. Self-supervised rewards might induce more general behaviours, inspiring the agent with an intrinsic desire to learn and explore the environment. In this work, we propose a curiosity-based bonus as intrinsic reward for Reinforcement Learning, computed as the bayesian surprise with respect to a latent dynamics model. We extensively evaluate our model by measuring the agent's performance in terms of environment exploration, for continuous tasks, and looking at the game scores achieved, for video games. Our model is computationally cheap and empirically shows state-of-the-art performance on several problems. We further corroborate the validity of our intrinsic bonus by performing an ablation study on an image-prediction task involving a stochastic dynamics, where our approach demonstrates to be the most resilient to simple stochastic actions.


### Arcade Games Experiments

The curves show the game score achieved during an episode of training by agents learning only using the intrinsic motivation signal.

They follow videos of the agents playing the games, driven only by their curiosity.

![Arcade Results](./resources/arcade_results.png)


##### BeamRider 
<video src="./resources/BeamRider-6140.mp4" width="480" height="360" controls preload></video>

##### Breakout 
<video src="./resources/Breakout-425.mp4" width="480" height="360" controls preload></video>

#### Montezuma Revenge
<video src="./resources/MontezumaRevenge-left-bugs.mp4" width="480" height="360" controls preload></video>

<video src="./resources/MontezumaRevenge-right-bugs.mp4" width="480" height="360" controls preload></video>

#### Pong
<video src="./resources/Pong-2-4.mp4" width="480" height="360" controls preload></video>

#### Qbert
<video src="./resources/Qbert-15600.mp4" width="480" height="360" controls preload></video>

#### Seaquest
<video src="./resources/Seaquest-1060.mp4" width="480" height="360" controls preload></video>

#### Space Invaders
<video src="./resources/SpaceInvaders-1370.mp4" width="480" height="360" controls preload></video>

#### Super Mario Bros.
<video src="./resources/MarioBros-pipe-world-1.mp4" width="480" height="360" controls preload></video>

<video src="./resources/MarioBros-all-world-1.mp4" width="480" height="360" controls preload></video>

