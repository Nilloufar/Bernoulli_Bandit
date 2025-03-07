# Task 3: Training a Simple Behavioral Cloning Model

## Objective
Train a simple behavioral cloning model using classical machine learning techniques to learn decision-making strategies from the p = 0.2 dataset that you split in Task 2.

## Background
Behavioral cloning is a form of imitation learning where an agent learns to perform a task by observing demonstrations. In this task, you'll use a simple classification model from scikit-learn to predict which arm (a₁ or a₂) to pull based on the observations in the Bernoulli bandit environment.

## Implementation Steps

1. **Load the Split Datasets**
- Load the training, validation, and test sets you created in Task 2:
 - `train_p0.2.csv`
 - `validation_p0.2.csv`
 - `test_p0.2.csv`


2. **Prepare Data:**
   - Separate the features (states) and labels (actions) for each dataset.
   - Example:
     ```python
     X_train = states of training set
     y_train = actions of training set
     ```

3. **Model Selection:**
   - Use `scikit-learn`'s `LogisticRegression` as the base model.

4. **Training:**
   - Train the logistic regression model on the training data (`X_train`, `y_train`).
   - Use the `fit()` method to learn the mapping from states to actions.

5. **Validation:**
   - Evaluate the model on the validation set (`X_val`, `y_val`).
   - Use metrics such as accuracy, precision, recall, or F1-score to measure performance.

6. **Final Evaluation:**
   - Evaluate the trained model on the test set (`X_test`, `y_test`).
   - Report the final performance metrics.

7. **Behavior Cloning:run the Environment for 10 Episodes:**

   - For each episode:
     - Reset the environment.
     - Use the trained model to select actions based on the current state.
     - Record the reward for each step.
     - Calculate the total reward for the episode.
     - Print the total reward for each episode.
8. **Compare:**
    - Compare the performance of the behavioral cloning model with the behavioral policy (policy that the data is obtained from) in terms of total rewards obtained.


