# Deep-RL-Sudoku
This project explores the use of reinforcement learning (RL) to solve Sudoku puzzles. It leverages the Gymnasium environment and Stable Baselines3 library to design and train RL agents such as DQN (Deep Q-Network) and PPO (Proximal Policy Optimization).

Methodology:
1. Dataset:
  - The project begins by loading a dataset of Sudoku puzzles, which is used to define the environment for the RL agents.
    
2. Environment Setup
  - The Gymnasium framework was utilized to create a custom environment for solving Sudoku puzzles. The environment is:
    •	State-Space Representation: A grid representing the Sudoku puzzle.
    •	Action-Space Representation: Possible moves or number placements.
    •	Reward Function: Designed to incentivize correct moves and penalize invalid actions.
    
3. Reinforcement Learning Agents
  - Two RL agents were implemented:
    •	DQN (Deep Q-Network): A model-free, off-policy algorithm using a neural network to approximate the Q-value function.
    •	PPO (Proximal Policy Optimization): A model-free, on-policy algorithm designed for better stability and sample efficiency.
    
4. Training Process
  - The training process includes:
    •	Wrapping the environment with monitoring tools like Monitor and DummyVecEnv.
    •	Using a GPU (CUDA device) for acceleration.
    •	Employing callbacks such as CheckpointCallback to save intermediate models.



Results:
  - Training Metrics:
    Key metrics observed during training include:
      •	Episode Length Mean: Averaging 2.25.
      •	Reward Mean: Averaging 2.82.
      •	Exploration Rate: Starting at 0.991 and reducing as the agent learns.
  - Performance Analysis:
    The RL agents demonstrated steady improvement in solving Sudoku puzzles, with a consistent decrease in episode length and an increase in rewards as training progressed.









Discussion:
Strengths
•	Efficient use of RL algorithms to approach a complex problem like Sudoku.
•	Effective integration of Gymnasium and Stable Baselines3 libraries.
•	GPU acceleration significantly enhanced training speed
