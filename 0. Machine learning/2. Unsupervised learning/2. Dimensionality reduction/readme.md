# ABOUT

- Dimensionality reduction is a way of converting the higher dimensions dataset into lesser dimensions dataset ensuring that it provides similar information.

- Handling the high-dimensional data is very difficult in practice, commonly known as the curse of dimensionality.

- If the dimensionality of the input dataset increases, any machine learning algorithm and model becomes more complex.

- There are two ways to apply the dimension reduction technique, which are given below:

## Feature Selection

- Feature selection is the process of selecting the subset of the relevant features and leaving out the irrelevant features present in a dataset to build a model of high accuracy.
- In other words, it is a way of selecting the optimal features from the input dataset.

- Three methods are used for the feature selection:

### Filters Methods

- In this method, the dataset is filtered, and a subset that contains only the relevant features is taken

**Some common techniques of filters method are:**

- Correlation
- Chi-Square Test
- ANOVA
- Information Gain, etc.

### Wrappers Methods

- The wrapper method has the same goal as the filter method, but it takes a machine learning model for its evaluation.
- In this method, some features are fed to the ML model, and evaluate the performance.
- The performance decides whether to add those features or remove to increase the accuracy of the model.
- This method is more accurate than the filtering method but complex to work.

**Some common techniques of wrapper methods are:**

- Forward Selection
- Backward Selection
- Bi-directional Elimination

### Embedded Methods:

- Embedded methods check the different training iterations of the machine learning model and evaluate the importance of each feature.

**Some common techniques of Embedded methods are:**

- LASSO
- Elastic Net
- Ridge Regression, etc.

## Feature Extraction:

- Feature extraction is the process of transforming the space containing many dimensions into space with fewer dimensions.
- This approach is useful when we want to keep the whole information but use fewer resources while processing the information.

**Some common feature extraction techniques are:**

- Principal Component Analysis
- Linear Discriminant Analysis
- Kernel PCA
- Quadratic Discriminant Analysis

## Common techniques of Dimensionality Reduction

**_Principal Component Analysis_**

- converts the observations of correlated features into a set of linearly uncorrelated features with the help of orthogonal transformation.
- These new transformed features are called the Principal Components.
- PCA works by considering the variance of each attribute because the high attribute shows the good split between the classes, and hence it reduces the dimensionality
- Some real-world applications of PCA are image processing, movie recommendation system, optimizing the power allocation in various communication channels.

- Backward Elimination
- Forward Selection
- Score comparison
- Missing Value Ratio
- Low Variance Filter
- High Correlation Filter
- Random Forest
- Factor Analysis
- Auto-Encoder

**_Benefits of applying Dimensionality Reduction_**

- By reducing the dimensions of the features, the space required to store the dataset also gets reduced.

- Less Computation training time is required for reduced dimensions of features.

- Reduced dimensions of features of the dataset help in visualizing the data quickly.

- It removes the redundant features (if present) by taking care of multicollinearity.

**_Disadvantages of dimensionality Reduction_**

- Some data may be lost due to dimensionality reduction.

- In the PCA dimensionality reduction technique, sometimes the principal components required to consider are unknown.

**Use cases**

- Meaningful compression
- Structure discovery
- Big data visualisation
- Feature elicitation
