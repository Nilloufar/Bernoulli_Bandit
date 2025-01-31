# Learning Optimal Decision Making with Two-Armed Bernoulli Bandits

## The Bernoulli Bandit Game 

The two-armed Bernoulli bandit represents a fundamental decision-making scenario where you must choose between two options (arms) with uncertain outcomes.

The game environment consists of:

* **Two Arms**: Called a₁ and a₂
* **Stochastic Rewards**: Each arm provides rewards following a Bernoulli distribution
  * Arm a₁: Gives reward 1 with probability (1-p), 0 otherwise
  * Arm a₂: Gives reward 1 with probability p, 0 otherwise
* **Optimal Strategy**: When p < 0.5, arm a₁ is optimal due to higher expected reward

### Example Scenario
Think of having two slot machines (we call them arms a₁ and a₂):
* When you pull arm a₁, you win $1 with probability (1-p)
* When you pull arm a₂, you win $1 with probability p
* Otherwise you get $0

When p = 0.3:
* Arm a₁ gives reward 1 with probability 0.7 (1-0.3)
* Arm a₂ gives reward 1 with probability 0.3

* The optimal strategy is to consistently choose a₁
___
## Objective:
* Create datasets by playing a simple two-choice game with random rewards
* Learn how to train an AI that copies successful playing strategies from these datasets
The goal is to teach an AI to make good decisions by learning from examples of past gameplay, just like how you might learn to play a game by watching someone else play!
___
## task 1: create dataset
