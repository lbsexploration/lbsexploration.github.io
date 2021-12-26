---
title: 'Curiosity-Driven Exploration<br>via Latent Bayesian Surprise'
---

## Abstract

> The human intrinsic desire to pursue knowledge, also known as curiosity, is considered essential in the process of skill acquisition. With the aid of artificial curiosity, we could equip current techniques for control, such as Reinforcement Learning, with more natural exploration capabilities. A promising approach in this respect has consisted of using Bayesian surprise on model parameters, i.e. a metric for the difference between prior and posterior beliefs, to favour exploration. In this contribution, we propose to apply Bayesian surprise in a latent space representing the agent’s current understanding of the dynamics of the system, drastically reducing the computational costs. We extensively evaluate our method by measuring the agent's performance in terms of environment exploration, for continuous tasks, and looking at the game scores achieved, for video games. Our model is computationally cheap and compares positively with current state-of-the-art methods on several problems. We also investigate the effects caused by stochasticity in the environment, which is often a failure case for curiosity-driven agents. In this regime, the results suggest that our approach is resilient to stochastic transitions.

### Visual Control Zero-shot Benchmark

This experiment evaluates the performance in a zero-shot learning setting (also see [Sekar et al. 2020](https://arxiv.org/abs/2005.05960) for details). 

The model and the agent are trained without rewards, collecting data through exploration. Some of the curiosity-driven behaviours learned in this phase with Latent Bayesian Surprise are showed in the GIF, under the <b>Exploration</b> column.

Along the exploration process, snapshots of the agent's model are used to train a task policy on the final task and plot its zero-shot performance. These behaviours are shown under the <b>Task</b> column.

<div class="row">
  <div class="column-2">
    <div><b>Exploration</b></div>
  </div>
  <div class="column-2">
    <div><b>Task</b></div>
  </div>
</div>
<br/>
<div class="row">
  <div class="column-2">
  <div class="column-3">
    <br/>
    <img src="./resources/dmc_gifs/acrobot_swingup_train.gif" alt="this slowpoke moves"  width="90%" />
  </div>
  </div>
  <div class="column-2">
    <div class="column-3">
        Acrobot Swingup
        <img src="./resources/dmc_gifs/acrobot_swingup_eval.gif" alt="this slowpoke moves"  width="90%" />
    </div>
  </div>
</div>
<br/>
<div class="row">
  <div class="column-2">
    <div class="column-3">
        <br/>
        <img src="./resources/dmc_gifs/cartpole_balance_train.gif" alt="this slowpoke moves"  width="90%" />
    </div>
  </div>
  <div class="column-2">
    <div class="column-3">
        Cartpole Balance
        <img src="./resources/dmc_gifs/cartpole_balance_eval.gif" alt="this slowpoke moves"  width="90%" />
    </div>
    <div class="column-3">
        Cartpole Swingup
        <img src="./resources/dmc_gifs/cartpole_swingup_eval.gif" alt="this slowpoke moves"  width="90%" />
    </div>
  </div>
</div>
<br/>
<div class="row">
  <div class="column-2">
    <div class="column-3">
        <br/>
        <img src="./resources/dmc_gifs/cheetah_run_train.gif" alt="this slowpoke moves"  width="90%" />
    </div>
  </div>
  <div class="column-2">
    <div class="column-3">
        Cheetah Run
        <img src="./resources/dmc_gifs/cheetah_run_eval.gif" alt="this slowpoke moves"  width="90%" />
    </div>
  </div>
</div>
<br/>
<div class="row">
  <div class="column-2">
    <div class="column-3">
        <br/>
        <img src="./resources/dmc_gifs/cup_catch_train.gif" alt="this slowpoke moves"  width="90%" />
    </div>
  </div>
  <div class="column-2">
    <div class="column-3">
        Cup Catch
        <img src="./resources/dmc_gifs/cup_catch_eval.gif" alt="this slowpoke moves"  width="90%" />
    </div>
  </div>
</div>
<br/>
<div class="row">
  <div class="column-2">
    <div class="column-3">
        <br/>
        <img src="./resources/dmc_gifs/finger_spin_train.gif" alt="this slowpoke moves"  width="90%" />
    </div>
    <div class="column-3">
        <br/>
        <img src="./resources/dmc_gifs/finger_turn_easy_train.gif" alt="this slowpoke moves"  width="90%" />
    </div>
    <div class="column-3">
        <br/>
        <img src="./resources/dmc_gifs/finger_turn_hard_train.gif" alt="this slowpoke moves"  width="90%" />
    </div>
  </div>
  <div class="column-2">
    <div class="column-3">
        Finger Spin
        <img src="./resources/dmc_gifs/finger_spin_eval.gif" alt="this slowpoke moves"  width="90%" />
    </div>
    <div class="column-3">
        Finger Turn Easy
        <img src="./resources/dmc_gifs/finger_turn_easy_eval.gif" alt="this slowpoke moves"  width="90%" />
    </div>
    <div class="column-3">
        Finger Turn Hard
        <img src="./resources/dmc_gifs/finger_turn_hard_eval.gif" alt="this slowpoke moves"  width="90%" />
    </div>
  </div>
</div>
<br/>
<div class="row">
  <div class="column-2">
    <div class="column-3">
        <br/>
        <img src="./resources/dmc_gifs/hopper_stand_train.gif" alt="this slowpoke moves"  width="90%" />
    </div>
  </div>
  <div class="column-2">
    <div class="column-3">
        Hopper Stand
        <img src="./resources/dmc_gifs/hopper_stand_eval.gif" alt="this slowpoke moves"  width="90%" />
    </div>
    <div class="column-3">
        Hopper Hop
        <img src="./resources/dmc_gifs/hopper_hop_eval.gif" alt="this slowpoke moves"  width="90%" />
    </div>
  </div>
</div>
<br/>
<div class="row">
  <div class="column-2">
    <div class="column-3">
        <br/>
        <img src="./resources/dmc_gifs/pendulum_swingup_train.gif" alt="this slowpoke moves"  width="90%" />
    </div>
  </div>
  <div class="column-2">
    <div class="column-3">
        Pendulum Swingup
        <img src="./resources/dmc_gifs/pendulum_swingup_eval.gif" alt="this slowpoke moves"  width="90%" />
    </div>
  </div>
</div>
<br/>
<div class="row">
  <div class="column-2">
    <div class="column-3">
        <br/>
        <img src="./resources/dmc_gifs/quadruped_run_train.gif" alt="this slowpoke moves"  width="90%" />
    </div>
  </div>
  <div class="column-2">
    <div class="column-3">
        Quadruped Walk
        <img src="./resources/dmc_gifs/quadruped_walk_eval.gif" alt="this slowpoke moves"  width="90%" />
    </div>
    <div class="column-3">
        Quadruped Run
        <img src="./resources/dmc_gifs/quadruped_run_eval.gif" alt="this slowpoke moves"  width="90%" />
    </div>    
  </div>
</div>
<br/>
<div class="row">
  <div class="column-2">
    <div class="column-3">
        <br/>
        <img src="./resources/dmc_gifs/reacher_easy_train.gif" alt="this slowpoke moves"  width="90%" />
    </div>
    <div class="column-3">
        <br/>
        <img src="./resources/dmc_gifs/reacher_hard_train.gif" alt="this slowpoke moves"  width="90%" />
    </div>
  </div>
  <div class="column-2">
    <div class="column-3">
        Reacher Easy
        <img src="./resources/dmc_gifs/reacher_easy_eval.gif" alt="this slowpoke moves"  width="90%" />
    </div>
    <div class="column-3">
        Reacher Hard
        <img src="./resources/dmc_gifs/reacher_hard_eval.gif" alt="this slowpoke moves"  width="90%" />
    </div>
  </div>
</div>
<br/>
<div class="row">
  <div class="column-2">
    <div class="column-3">
        <br/>
        <img src="./resources/dmc_gifs/walker_walk_train.gif" alt="this slowpoke moves"  width="90%" />
    </div>
  </div>
  <div class="column-2">
    <div class="column-3">
        Walker Stand
        <img src="./resources/dmc_gifs/walker_stand_eval.gif" alt="this slowpoke moves"  width="90%" />
    </div>
    <div class="column-3">
        Walker Walk
        <img src="./resources/dmc_gifs/walker_walk_eval.gif" alt="this slowpoke moves"  width="90%" />
    </div>
    <div class="column-3">
        Walker Run
        <img src="./resources/dmc_gifs/walker_run_eval.gif" alt="this slowpoke moves"  width="90%" />
    </div>
  </div>
</div>

### Arcade Games Experiments

The curves show the game score achieved during an episode of training. Agents learn using only the intrinsic motivation signal.


<div style='text-align: center'>
    <img src="./resources/arcade_results.png" alt="Arcade Results" width="100%">
</div>

To incentivize comparison against our baseline, we make public the data used in the plots, which can be easily integrated with the original [Large-Scale Study of Curiosity-Driven Learning](https://github.com/openai/large-scale-curiosity) open-source implementation.

<a href="/resources/lbs_arcade_results.zip" download>Download Data [.zip]</a>

They follow videos of the agents playing the games, driven only by their curiosity.

<div class="row">
    <div class="column-4" style='text-align: center'>
    <h4> BeamRider </h4> 
        <video style=' background-color: rgba(0, 0, 0, 0)' src="./resources/BeamRider-6140.mp4" width="90%" controls preload></video>
    </div>
    <div class="column-4" style='text-align: center'>
    <h4> Breakout </h4> 
        <video style=' background-color: rgba(0, 0, 0, 0)' src="./resources/Breakout-425.mp4" width="90%" controls preload></video>
    </div>
    <div class="column-4" style='text-align: center'>
    <h4> Montezuma Revenge</h4> 
        <video style=' background-color: rgba(0, 0, 0, 0)' src="./resources/MontezumaRevenge-1400.mp4" width="90%" controls preload></video>
    </div>
    <div class="column-4" style='text-align: center'>
    <h4> Pong </h4>
        <video style=' background-color: rgba(0, 0, 0, 0)' src="./resources/Pong-2-4.mp4" width="90%" controls preload></video>
    </div>
</div>
<div class="row">
    <div class="column-4" style='text-align: center'>
        <h4> Qbert </h4>
        <video style=' background-color: rgba(0, 0, 0, 0)' src="./resources/Qbert-15600.mp4" width="90%" controls preload></video>
    </div>
    <div class="column-4" style='text-align: center'>
        <h4> Riverraid</h4>
        <video style=' background-color: rgba(0, 0, 0, 0)' src="./resources/Riverraid-6890.mp4" width="90%" controls preload></video>
    </div>
    <div class="column-4" style='text-align: center'>
        <h4> Seaquest</h4>
        <video style=' background-color: rgba(0, 0, 0, 0)' src="./resources/Seaquest-1060.mp4" width="90%" controls preload></video>
    </div>
    <div class="column-4" style='text-align: center'>
        <h4> Space Invaders</h4>
        <video style=' background-color: rgba(0, 0, 0, 0)' src="./resources/SpaceInvaders-1370.mp4" width="90%" controls preload></video>
    </div>
</div>
<h4> Super Mario Bros.</h4>
<div class="row">
    <div class="column-4" style='text-align: center'></div>
    <div class="column-4" style='text-align: center'>
        <video style=' background-color: rgba(0, 0, 0, 0)' src="./resources/MarioBros-pipe-world-1.mp4" width="90%" controls preload></video>
    </div>
    <div class="column-4" style='text-align: center'>
        <video style=' background-color: rgba(0, 0, 0, 0)' src="./resources/MarioBros-all-world-1.mp4" width="90%" controls preload></video>
    </div>
    <div class="column-4" style='text-align: center'></div>
</div>
