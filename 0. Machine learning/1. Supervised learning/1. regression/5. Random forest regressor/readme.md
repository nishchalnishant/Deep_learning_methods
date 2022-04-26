## About --

- It builds decision trees on different samples and takes their majority vote for classification and average in case of regression.

- It performs better results for classification problems, but it can handle the dataset containing continous variables as in the case of regression.

# Important terms related to random forest

**_Bagging_**

- Also known as bootstrap aggregation.
- It creates a different training subset from sample training data with replacement & the final output is based on majority voting. For example, Random Forest.

**_Boosting_**

- It combines weak learners into strong learners by creating sequential models such that the final model has the highest accuracy. For example, ADA BOOST, XG BOOST

# Steps involved in random forest algorithm:

Step 1: In Random forest n number of random records are taken from the data set having k number of records.

Step 2: Individual decision trees are constructed for each sample.

Step 3: Each decision tree will generate an output.

Step 4: Final output is considered based on Majority Voting or Averaging for Classification and regression respectively.

- **Pros:**

- Robust to outliers.
- Works well for non-linear data.
- Low risk of overfitting.
- Runs efficiently on large datasets.

**Cons:**

- Slow training.
- Biased when dealing with categorical variables.
