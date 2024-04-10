---
title: "Combining Reinforcement Learning and Evolutionary Strategies in Tetris"
excerpt: "Developed a Tetris environment to compare the performance of Deep Q learning with the cross entropy method. We then propose a novel approach that combines the strenghts of both algorithms."
collection: portfolio
---

## Project Goal
This project trained an agent to clear as many lines in Tetris using Deep Q networks and the Cross entropy method. Tetris is a classical puzzle game that provides an ideal testing ground for comparing the effectiveness of reinforcement learning and evolutionary strategies. To accomplish our aim we:

- **Develop a Tetris Environment:**  We create a Tetris environment for analysis.
- **Implement and Evaluate CE:** We implement the CE method in Tetris and compare
the effect of adding noise. We observe fast convergence to a good policy that clears
three times more lines than DQN on the 10x10 grid.
- **Implement and Evaluate DQN:** We implement DQN in Tetris with a replay buffer,
target network and decaying epsilon greedy policy. Our results show steady improvement
in performance and highlight DQN’s sensitivity to hyper-parameters in Tetris.
- **Combine DQN and CE:** Building on the strengths of policy based (CE) and value
based (DQN) methods, we use CE’s direct policy search to identify promising solutions.
Then, we use DQN’s iterative updates to fine-tune the policy with the ultimate goal of
clearing more lines. We observe limited learning

<p align="center">
  <img src="https://github.com/SirSebLancelot/Tetris-Reinforcement-Learning/raw/main/dqn_results/results20x10/tetris_animation_looped_long.gif" alt="Tetris Animation" />
</p>

## Results:

There are 3 folders containing the results from training each of the 3 agents:
`ce_results`, `dqn_results`, and `combine_results`. These contain the trained agent
networks and storing the rewards for plotting.

The performance of an agent was visualised by comparing the number of lines for each agent. Below is an example of the DQN agent compared on the 6x5 and 10x10 grid:
<p align="center">
  <img src= 'https://github.com/SJackson123/Tetris-Reinforcement-Learning/blob/main/dqn_results/compare_DQN.png?raw=true' alt="Tetris Animation" />
</p>
