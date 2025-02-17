## Task 2: Train-Test-Validation Split for \( p = 0.2 \)

### Objective
Split the dataset generated for \( p = 0.2 \) into **training**, **testing**, and **validation** sets. This prepares the data for training and evaluating an AI model in subsequent tasks.

---

### Steps

#### 1. Load the Dataset for \( p = 0.2 \)
- Load the dataset generated in Task 1 for \( p = 0.2 \).
- The dataset should include:
  - The chosen arm (a₁ or a₂).
  - The reward received (0 or 1).

#### 2. Split the Dataset
- Divide the dataset into three subsets:
  - **Training Set**: 70% of the data.
  - **Validation Set**: 15% of the data.
  - **Test Set**: 15% of the data.
  
- You can use the `train_test_split` function from the `sklearn.model_selection` module to perform the splits.
- Ensure to set a random seed (e.g., `random_state=42`)

#### 3. Verify the Splits
- Check that the distribution of rewards (0s and 1s) is similar across the training, validation, and test sets.
- Calculate the average reward for each subset to ensure consistency.

#### 4. Save the Splits
- Save the training, validation, and test sets as separate files (e.g., CSV or NumPy arrays) for future use.

---

### Deliverables
1. A Python script or notebook that performs the train-test-validation split for \( p = 0.2 \).
2. Three datasets saved as files:
   - `train_p0.2.csv`
   - `validation_p0.2.csv`
   - `test_p0.2.csv`
3. A summary of the dataset statistics (e.g., size of each split, average reward in each subset).

---

