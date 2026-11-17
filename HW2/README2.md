
# A/B Testing - Epsilon-Greedy and Thompson Sampling

## Overview

This assignment compares two multi-armed bandit algorithms:
- Epsilon-Greedy with epsilon decay of 1/t.
- Thompson Sampling with known reward precision.

## Experiment Setup

- Number of advertisements: 4
- True reward values: [1, 2, 3, 4]
- Number of trials: 20,000 per algorithm
- Reward distribution: Normal distribution
- Reward precision: 1

## Implementation

The experiment implements:
- An abstract Bandit class.
- EpsilonGreedy class.
- ThompsonSampling class.
- Visualization of estimated rewards.
- Comparison of cumulative rewards and cumulative regrets.

## Results

Both algorithms learned to select Advertisement 4, which has the highest expected reward.

In the completed run:
- Epsilon-Greedy cumulative reward: 79,734.47
- Thompson Sampling cumulative reward: 79,369.13
- Epsilon-Greedy cumulative regret: 135
- Thompson Sampling cumulative regret: 598

These results correspond to one experimental run and may vary because of random sampling.

## Files

- A_B_Testing.ipynb: Complete implementation and visualizations.
- bandit_results.csv: Combined experimental results.
- epsilon_greedy_results.csv: Epsilon-Greedy results.
- thompson_sampling_results.csv: Thompson Sampling results.
- requirements.txt: Required Python packages.
