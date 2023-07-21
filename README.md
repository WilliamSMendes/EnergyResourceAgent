# Energy Saving Environment
This repository contains a customized reinforcement learning environment called "EnergySavingEnv" to simulate an energy management scenario. The environment is designed to allow an agent to learn to make decisions to save energy efficiently over time.

## Description
The "EnergySavingEnv" environment is a customized environment based on OpenAI Gym and simulates an energy manager. The goal is for the agent to learn to take actions to increase, decrease, or maintain its energy level, so as to maximize its cumulative rewards over time.

## Observation
The environment has a single observation representing the current energy level. The energy level varies between 0 and 100.

## Action space
The action space is discrete and consists of three possible actions:

-1: Decrease energy level.
0: Maintain energy level (do nothing).
1: Increase the energy level.

## Resources to be managemented
The agent must manage the energy level to keep it close to or above an energy saving threshold. The environment has the following resources to manage:

* Maximum energy capacity: 100 units
* Energy saving threshold: 60 units
* Energy saving factor: 0.5 (represents the percentage of energy saved when in saving mode)
* Energy use per time step: 5 units


## Reward
The agent's reward is based on the efficiency of energy management. If the energy level is above the energy saving threshold, the agent will receive a positive reward (1). Otherwise, the agent will receive a negative reward (-1).

## Episode time
Each episode of the environment has a fixed time of 100 steps. The episode will end after 100 time steps.

## Results
![The mean reward](https://github.com/WilliamSMendes/EnergyResourceAgent/assets/57918792/6cc58893-b0e0-427f-9589-1fce6eba36fb)
![fps](https://github.com/WilliamSMendes/EnergyResourceAgent/assets/57918792/f3b9ba70-3a98-46f7-8c0a-990caf66d562)


# Others projects
This repository also contains other projects that utilize OpenAI's Gym to create reinforcement learning agents in different scenarios:

* Atari Agent: A reinforcement learning agent for playing Atari games using the Atari Gym environment.

* Self-Driving Agent: A reinforcement learning agent for piloting an autonomous car in simulated environments.

* Lunar Lander Agent: A reinforcement learning agent for solving the lunar landing problem using Gym's LunarLander environment.

* Blackjack Agent: A reinforcement learning agent for playing Blackjack (21) using Gym's Blackjack environment.

Feel free to explore each of these projects and learn more about how reinforcement learning can be applied in different problem scenarios.

# References
* OpenAI Gym: https://gymnasium.farama.org/
* Reinforcement Learning: An Introduction by Richard S. Sutton and Andrew G. Barto
