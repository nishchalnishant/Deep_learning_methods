# About --

- KNN can be used for both classification and regression predictive problems

> The algorithm’s learning is:

- Instance-based learning: Here we do not learn weights from training data to predict output (as in model-based algorithms) but use entire training instances to predict output for unseen data.

- Lazy Learning: Model is not learned using training data prior and the learning process is postponed to a time when prediction is requested on the new instance.

- Non -Parametric: In KNN, there is no predefined form of the mapping function.

# How does KNN Work?

- nearest neighbors are those data points that have minimum distance in feature space from our new data point.

- And K is the number of such data points we consider in our implementation of the algorithm.

- Therefore, distance metric and K value are two important considerations while using the KNN algorithm.

- For predicting class/ continuous value for a new data point, it considers all the data points in the training dataset.

- Finds new data point’s ‘K’ Nearest Neighbors (Data points) from feature space and their class labels or continuous values.

- For regression: Mean or median of continuous values assigned to K Nearest Neighbors from training dataset is a predicted continuous value for our new data point

**_Pros:_**

- Easy to understand, implement, and explain.
- Is a non-parametric algorithm, so does not have strict assumptions.
- No training steps are required. It uses training data at run time to make predictions making it faster than all those algorithms that need to be trained.
- Since it doesn’t need training on the train data, data points can be easily added.

**_Cons:_**

- Inefficient and slow when the dataset is large. As for the cost of the calculation, the distance between the new point and train points is high.
- Doesn’t work well with high dimensional data because it becomes harder to find the distance in higher dimensions.
- Sensitive to outliers, as it is easily affected by outliers.
- Cannot work when data is missing. So data needs to be manually imputed to make it work.
- Needs feature scaling/normalization.
