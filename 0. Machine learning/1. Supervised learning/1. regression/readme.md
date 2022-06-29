## Metrics that can be used for regression techniques --

**Mean absolute error (MAE)**

- Sum of all errors and divide them by a total number of observations.
- MAE measures the average magnitude of the errors in a set of forecasts, without considering their direction.
- It measures accuracy for continuous variables.
- MAE is a linear score which means that all the individual differences are weighted equally in the average.

**mean squared error (MSE)**

- Sum of all errors squared and dividing them by total number of observations.
- Mean squared error (MSE) tells us how close a regression line is to a set of points.
- It does this by taking the distances from the points to the regression line (these distances are the “errors”) and squaring them.
- The squaring is necessary to remove any negative signs.
- Smaller the mean squared error, the closer you are to finding the line of best fit.

**Root mean squared error (RMSE)**

- Square root of mean squared error.
- Root Mean Square Error (RMSE) is the standard deviation of the residuals (prediction errors).
- Residuals are a measure of how far from the regression line data points are; RMSE is a measure of how spread out these residuals are.
- RMSE can be thought of as some kind of (normalized) distance between the vector of predicted values and the vector of observed values.

**R squared**

- Also known as coefficient of determination, used to explain the degree to which input variables explain the variation of output variables.
- Ranges from 0 to 1.
- A higher R-squared indicates a better fit for the model.
- Squared sum error of regression line
- There is one problem with R-squared that even if the additional input variables show no relationship with the output variables, the R-squared will increase.
- To overcome above problem we introduced Adjusted R-Squared.

**Adjusted R squares**

- Modified version of R-Squared that shows whether adding additional predictors improve a regression model or not.
- Compared to a model with additional input variables, a lower adjusted R-squared indicates that the additional input variables are not adding value to the model.
- Compared to a model with additional input variables, a higher adjusted R-squared indicates that the additional input variables are adding value to the model.

## Algorithms for regression --

**Linear regression**

- Assumes linear relationship between the input variables and single ouput variables .
- There are various methods to fit the linear regression from the data , most common of which is Ordinary least squares.
- We can fit the linear regression model using simple linear regression ,ordinary lelast squares, Gradient descent and regularizations (L1 lasso and L2 ridge)

> Assumptions --

- variables should be measured at a continuous level
- The data should have no significant outliers.
- Check for homoscedasticity — a statistical concept in which the variances along the best-fit linear-regression line remain similar all through that line.
- The residuals (errors) of the best-fit regression line follow normal distribution.

**Support vector machines**

- Can be used in regression as well as for classification
- Objective is to find a hyperplane in a n dimensional space that distinctly classifies the data points .
- If we are unable to split the datset using 2 dimensional hyper plane ,we move onto to the 3 dimensional hyperplane till we suceed.

> Assumptions:

- It assumes data is independent and identically distributed.

**Descision tree**

- Can be used to solve regression and classification problems.
- It breaks down a dataset into smaller and smaller subsets while at the same time an associated decision tree is incrementally developed.
- The final result is a tree with decision nodes and leaf nodes.
- We start from root of the tree and compare the root attribute with the record attribute, on the basis of comparison we follow the branch corresponding to that value and jump to the next node.

> Assumptions:

- Initially, whole training data is considered as root.
- Records are distributed recursively on the basis of the attribute value.

> Basic terminology used with decision trees:

- Root Node: It represents entire population or sample and this further gets divided into two or more homogeneous sets.
- Splitting: It is a process of dividing a node into two or more sub-nodes.
- Decision Node: When a sub-node splits into further sub-nodes, then it is called decision node.
- Leaf/Terminal Node: Nodes do not split is called Leaf or Terminal node.
- Pruning: When we remove sub-nodes of a decision node, this process is called pruning. You can say opposite process of splitting.
- Branch / Sub-Tree: A sub section of entire tree is called branch or sub-tree.
- Parent and Child Node: A node, which is divided into sub-nodes is called parent node of sub-nodes whereas sub-nodes are the child of parent node.

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/descision_tree_regression.jpg?raw=true)

**Random forest**

- Random forest is a supervised ensemble learning algorithm that is used for both classifications as well as regression problems.
- But however, it is mainly used for classification problems.
- The random forest algorithm creates decision trees on data samples and then gets the prediction from each of them and finally selects the best solution by means of voting.
- It is an ensemble method that is better than a single decision tree because it reduces the over-fitting by averaging the result.

> Assumption

- Assumption of no formal distributions. Being a non-parametric model, it can handle skewed and multi-modal data.

**K nearest neighbours**

- K-Nearest Neighbour is one of the simplest Machine Learning algorithms based on Supervised Learning technique.
- K-NN algorithm assumes the similarity between the new case/data and available cases and put the new case into the category that is most similar to the available categories.
- K-NN algorithm stores all the available data and classifies a new data point based on the similarity.
- This means when new data appears then it can be easily classified into a well suite category by using K- NN algorithm.
- K-NN algorithm can be used for Regression as well as for Classification but mostly it is used for the Classification problems.
- K-NN is a non-parametric algorithm, which means it does not make any assumption on underlying data.
- It is also called a lazy learner algorithm because it does not learn from the training set immediately instead it stores the dataset and at the time of classification, it performs an action on the dataset.
- KNN algorithm at the training phase just stores the dataset and when it gets new data, then it classifies that data into a category that is much similar to the new data.
- Example: Suppose, we have an image of a creature that looks similar to cat and dog, but we want to know either it is a cat or dog. So for this identification, we can use the KNN algorithm, as it works on a similarity measure. Our KNN model will find the similar features of the new data set to the cats and dogs images and based on the most similar features it will put it in either cat or dog category.

> Assumptions:

- The data is in feature space, which means data in feature space can be measured by distance metrics such as Manhattan, Euclidean, etc.
- Each of the training data points consists of a set of vectors and a class label associated with each vector.
- Desired to have ‘K’ as an odd number in case of 2 class classification.

## Use cases of regression

- Population growth prediction
- Advertising popularity prediction
- Weather forecasting
- Market forecasting
- Estimating life expectancy
