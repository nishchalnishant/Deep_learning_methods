## Principal Component Analysis

- Principal Component Analysis(PCA) is one of the most popular linear dimension reduction

- PCA is a projection based method which transforms the data by projecting it onto a set of orthogonal axes.

- PCA finds best linear combinations of the original variables so that the variance or spread along the new variable is maximum.

### Advantages of Principal Component Analysis

**1. Removes Correlated Features:**

- In a real-world scenario, this is very common that you get thousands of features in your dataset.
- We cannot run your algorithm on all the features as it will reduce the performance of your algorithm and it will not be easy to visualize that many features in any kind of graph.
- So, we MUST reduce the number of features in your dataset.
- We need to find out the correlation among the features (correlated variables).
- Finding correlation manually in thousands of features is nearly impossible, frustrating and time-consuming.
- PCA does this for us efficiently.
- After implementing the PCA on your dataset, all the Principal Components are independent of one another.
- There is no correlation among them.

**2. Improves Algorithm Performance:**

- With so many features, the performance of your algorithm will drastically degrade.
- PCA is a very common way to speed up your Machine Learning algorithm by getting rid of correlated variables which don’t contribute in any decision making.
- The training time of the algorithms reduces significantly with less number of features.
- So, if the input dimensions are too high, then using PCA to speed up the algorithm is a reasonable choice.

**3. Reduces Overfitting:**

- Overfitting mainly occurs when there are too many variables in the dataset.
- So, PCA helps in overcoming the overfitting issue by reducing the number of features.

**4. Improves Visualization:**

- It is very hard to visualize and understand the data in high dimensions.
- PCA transforms a high dimensional data to low dimensional data (2 dimension) so that it can be visualized easily.
- We can use 2D Scree Plot to see which Principal Components result in high variance and have more impact as compared to other Principal Components.
- Even the simplest IRIS dataset is 4 dimensional which is hard to visualize. We can use PCA to reduce it to 2-dimension for better visualization.

## Disadvantages of Principal Component Analysis

**1. Independent variables become less interpretable:**

- After implementing PCA on the dataset, our original features will turn into Principal Components.
- Principal Components are the linear combination of your original features.
- Principal Components are not as readable and interpretable as original features.

**2. Data standardization is must before PCA:**

- You must standardize your data before implementing PCA, otherwise PCA will not be able to find the optimal Principal Components.
- For instance, if a feature set has data expressed in units of Kilograms, Light years, or Millions, the variance scale is huge in the training set.
- If PCA is applied on such a feature set, the resultant loadings for features with high variance will also be large.
- Hence, principal components will be biased towards features with high variance, leading to false results.
- Also, for standardization, all the categorical features are required to be converted into numerical features before PCA can be applied.
- PCA is affected by scale, so you need to scale the features in your data before applying PCA.

**3. Information Loss:**

- Although Principal Components try to cover maximum variance among the features in a dataset, if we don’t select the number of Principal Components with care, it may miss some information as compared to the original list of features.
