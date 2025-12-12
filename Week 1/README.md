# Week 1 — Multi-Armed Bandits

You have your toolkit ready; now it is time to dive into reinforcement learning. Week 1 introduces the exploration–exploitation dilemma through classic multi-armed bandit problems.

## Objectives

- Understand the ε-greedy strategy and why pure greed fails.
- Implement and compare multiple bandit strategies.
- Build plots and tables that communicate algorithm behaviour.
- Reflect on what exploration means in larger RL settings.

## Prerequisites

- Week 0 setup complete (working virtual environment + Jupyter).
- Chapter 2 of Sutton & Barto read or skimmed (`Resources/Reinforcement Learning - Sutton and Barto.pdf`).
- Comfort running the warm-up notebooks.

## Suggested workflow

1. **Read** Chapter 2 (up to and including Section 2.5) focusing on the k-armed bandit example.
2. **Browse** `bandits.py` to understand the helper functions and the experiment harness.
3. **Open** `work_on_bandits.ipynb` and duplicate it (e.g. `work_on_bandits_yourname.ipynb`) so you can track your version.
4. **Implement** the following agents inside the notebook or `bandits.py`:
   - Greedy action selection.
   - ε-greedy with constant ε (e.g. 0.1).
   - (Stretch) Decaying ε schedule or optimistic initialisation.
5. **Experiment** with different step sizes, horizons, and reward distributions. Log at least one surprise from your runs.
6. **Visualise** average reward and optimal action percentage over time using Matplotlib.

## Deliverables

- Code or notebook showing your implementations and experiments.
- Plots comparing at least two strategies on the same problem instance.


## Extensions

- Try the Upper Confidence Bound (UCB1) algorithm and compare with ε-greedy.
- Implement a simple Thompson Sampling agent for Gaussian bandits.
- Build a command-line interface using `bandits.py` to run experiments quickly.

## Tips

- Keep experiments reproducible by setting a random seed.
- Use tqdm or print statements sparingly to avoid slowing down large runs.


Once you are comfortable with bandits, you are ready for Week 2 where Markov decision processes and dynamic programming await.
