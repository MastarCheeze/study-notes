# Model-based and Model-free RL

`reinforcement learning`

## Model\-based RL

The agent predicts what will happen in the environment before taking any action. The agent builds an explicit representation of the environment \(**model**\) it interacts with. This model includes information about the **transition** dynamics \(how the environment state changes in response to actions\) and the **reward** structure \(the immediate rewards associated with state\-action pairs\). The agent then uses this learned model to simulate different scenarios and plan its actions.

## Model\-free RL

The agent doesn't explicitly learn a model of the environment. Instead, it focuses on learning a **policy** \(a mapping from states to actions\) or a **value function** \(an estimate of the expected cumulative reward from a given state\).
