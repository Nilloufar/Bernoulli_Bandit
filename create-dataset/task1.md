## Task 1: Generate Training Datasets

Create multiple datasets that capture different scenarios of this decision-making problem by varying the probability parameter p.
### Implementation Steps

1. Generate 5 separate datasets using these probability values:
   * p = 0.1 
   * p = 0.2
   * p = 0.3
   * p = 0.4
   * p = 0.5

2. Use the provided code structure:

```python
# Example for generating one dataset
env = BernoulliBanditEnv(bernoulli_prob=p)
env = BernoulliBanditWrapper(env)
get_bandit_dataset(env, p=p, N_steps=10000)
```

### Analyzing Your Datasets

After collecting the data, let's calculate the average rewards to understand how well different strategies work.

Create a table like this and fill it in with your results:

| p value | Expected Reward a₁ | Expected Reward a₂ | Average Reward in Dataset |
|---------|-------------------|-------------------|------------------------|
| 0.1     | 0.9 (1-0.1)      | 0.1              | [calculate from data] |
| 0.2     | 0.8 (1-0.2)      | 0.2              | [calculate from data] |
| 0.3     | 0.7 (1-0.3)      | 0.3              | [calculate from data] |
| 0.4     | 0.6 (1-0.4)      | 0.4              | [calculate from data] |
| 0.5     | 0.5 (1-0.5)      | 0.5              | [calculate from data] |


### Visualizing the Results

After collecting your datasets, create a plot to visualize how rewards change with different probability values:

#### Plot Components:

**X-axis (Probability p)**
* Shows p values from 0.1 to 0.5
* These are the different probabilities we tested

**Y-axis (Average Reward)**
* Shows average rewards from collected data


**Lines to Include:**
1. Line for actual collected data (what you measured)
2. Line for optimal policy (policy that always takes a₁ theoretical reward) of arm a₁ [x=p , y=(1-p)]



