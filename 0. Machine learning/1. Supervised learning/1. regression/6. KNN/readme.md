**Pros:**

- Easy to understand, implement, and explain.
- Is a non-parametric algorithm, so does not have strict assumptions.
- No training steps are required. It uses training data at run time to make predictions making it faster than all those algorithms that need to be trained.
- Since it doesn’t need training on the train data, data points can be easily added.

**Cons:**

- Inefficient and slow when the dataset is large. As for the cost of the calculation, the distance between the new point and train points is high.
- Doesn’t work well with high dimensional data because it becomes harder to find the distance in higher dimensions.
  Sensitive to outliers, as it is easily affected by outliers.
- Cannot work when data is missing. So data needs to be manually imputed to make it work.
- Needs feature scaling/normalization.
