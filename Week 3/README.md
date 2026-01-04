# Week 3 — Dynamic Programming Projects

Week 3 brings together everything you have practised so far. You will implement policy iteration and value iteration for two classic reinforcement learning problems from Sutton & Barto, analyse the resulting policies, and communicate your findings with clear visuals.

## Objectives

- Apply dynamic programming (DP) algorithms to larger, structured MDPs.
- Diagnose convergence behaviour and tune stopping criteria.
- Visualise optimal policies/value functions and interpret what they mean.
- Relate modelling assumptions (rewards, constraints) to the resulting strategy.

## Prerequisites

- Week 2 notebook complete—you can comfortably express an MDP and run value updates.
- Sutton & Barto Chapter 4 read or skimmed (policy evaluation, policy iteration, value iteration).
- Optional: David Silver’s [lecture on policy iteration](https://www.youtube.com/watch?v=_j6pvGEchWU) for an additional walkthrough.

## Assignments

1. **Jack’s Car Rental** (`Assignments/`)  
   - Revisit Example 4.2 in Sutton & Barto and note the state/action definition.  
   - Implement policy iteration (policy evaluation + improvement) to find the optimal overnight transfer policy.  
   - Visualise the final policy as a heatmap. Use `Assignments/image.png` as a reference output if helpful.

2. **Gambler’s Problem** (`More Assignments/`)  
   - Translate Example 4.3 into code: states are capital levels; actions are stakes.  
   - Run value iteration until convergence and extract the optimal stake for each capital level.  
   - Plot the optimal policy as a bar chart and describe any surprising jumps or plateaus.

## Suggested workflow

1. **Plan** — write down state/action spaces, reward structure, and terminal conditions for each problem.  
2. **Implement** — code policy iteration or value iteration loops with a convergence threshold (e.g. `delta < 1e-4`).  
3. **Track progress** — log the maximum value change each iteration to confirm convergence behaviour.  
4. **Visualise** — produce heatmaps/line plots that communicate the policy clearly; annotate axes so others can interpret them.  

## Deliverables

- Completed notebooks or scripts for both assignments.  
- Plots showing the optimal policy (and optionally value functions) for each task.  

## Extensions

- Introduce stochastic demand or extra rental bonuses in Jack’s Car Rental and observe policy changes.  
- Experiment with different reward targets or success probabilities in Gambler’s Problem.  
- Present a short demo to the cohort summarising your methodology and takeaways.

## Looking ahead

With dynamic programming under your belt, you are ready to explore Monte Carlo and temporal-difference methods, or start building agents in simulation environments like OpenAI Gym. Capture ideas for future experiments in a shared doc so the next cohort can build on your momentum.