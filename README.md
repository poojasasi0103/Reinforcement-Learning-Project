# Reinforcement Learning Project

## Assignment 1: Windy Gridworld using Sarsa

### Objective
Implementation of the Windy Gridworld problem (Example 6.5) using the ε-greedy Sarsa algorithm.

The objective is to train an agent to learn an efficient path from the starting state to the goal while considering the upward wind in the environment.

### Problem Description
The Windy Gridworld environment consists of a 7 × 10 grid.

- **Start State:** (3, 0)
- **Goal State:** (3, 7)
- **Actions:** UP, DOWN, LEFT, RIGHT
- **Wind Strength:** [0, 0, 0, 1, 1, 1, 2, 2, 1, 0]
- **Reward:** -1 for each normal time step and 0 when the goal is reached.

### Algorithm Used
**Sarsa (On-Policy Temporal Difference Learning)**

The agent uses an ε-greedy policy to balance exploration and exploitation.

Sarsa update equation:

Q(S,A) ← Q(S,A) + α[R + γQ(S',A') − Q(S,A)]

### Parameters

| Parameter | Value |
|---|---|
| Learning Rate (α) | 0.5 |
| Discount Factor (γ) | 1.0 |
| Exploration Rate (ε) | 0.1 |
| Training Time Steps | 8000 |
| Grid Size | 7 × 10 |

### Technologies Used
- Python
- NumPy
- Matplotlib
- Jupyter Notebook

### How to Run
1. Download or clone this repository.
2. Open the `.ipynb` file using Jupyter Notebook or Google Colab.
3. Run all cells sequentially.
4. Observe the agent's learning process and the learned greedy policy.

### Repository Contents
- `RL_assignement_1_wind_grid (1).ipynb` – Implementation and explanation of the Windy Gridworld problem using ε-greedy Sarsa.
- `README.md` – Project description and instructions.

### Expected Outcome
The agent learns to navigate the Windy Gridworld environment from the start state to the goal state while compensating for the upward wind.

The learned greedy policy demonstrates how Sarsa improves action selection through experience.

---

**Coursework:** Reinforcement Learning  
**Assignment:** Part I – Implementation of Book Examples
