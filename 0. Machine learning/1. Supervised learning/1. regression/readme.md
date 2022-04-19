**Use cases**

- Population growth prediction
- Advertising popularity prediction
- Weather forecasting
- Market forecasting
- Estimating life expectancy

## Metrics that can be used for regression techniques --

**mean absolute error (MAE)**

- sum of all errors and divide them by a total number of observations.

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/mae.jpg?raw=true)

**mean squared error (MSE)**

- Sum of all errors squared and dividing them by total number of observations.

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/mse.jpg?raw=true)

**Root mean squared error (RMSE)**

- Square root of mean squared error

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/rmse.jpg?raw=true)

**R squared**

- 1-(SSr/SSm)
- Squared sum error of regression line
- Squared sum error of mean line

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/r_squared.jpg?raw=true)

**Adjusted R squares**

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/regression.png?raw=true)

## Algorithms for regression --

**Linear regression**

- Assumes linear relationship between the input variables and single ouptu variables .
- There are various methods to fit the linear regression from the data , most common of which is Ordinary least squares.
- We can fit the linear regression model using simple linear regression ,ordinary lelast squares, Gradient descent and regularizations (L1 lasso and L2 ridge)

**Support vector machines**

- can be used in regression as well as for classification
- Objective is to find a hyperplane in a n dimensional space that distinctly classifies the data points .
- If we are unable to split the datset using 2 dimensional hyper plane ,we move onto to the 3 dimensional hyperplane till we suceed.

**Descision tree**

- Can be used to solve regression and classification problems.
- It breaks down a dataset into smaller and smaller subsets while at the same time an associated decision tree is incrementally developed.
- The final result is a tree with decision nodes and leaf nodes.
- We start from root of the tree and compare the root attribute with the record attribute, on the basis of comparison we follow the branch corresponding to that value and jump to the next node.
- basic terminology used with decision trees:

- - Root Node: It represents entire population or sample and this further gets divided into two or more homogeneous sets.
- - Splitting: It is a process of dividing a node into two or more sub-nodes.
- - Decision Node: When a sub-node splits into further sub-nodes, then it is called decision node.
- - Leaf/Terminal Node: Nodes do not split is called Leaf or Terminal node.
- - Pruning: When we remove sub-nodes of a decision node, this process is called pruning. You can say opposite process of splitting.
- - Branch / Sub-Tree: A sub section of entire tree is called branch or sub-tree.
- - Parent and Child Node: A node, which is divided into sub-nodes is called parent node of sub-nodes whereas sub-nodes are the child of parent node.

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/descision_tree_regression.jpg?raw=true)

**Random forest**

- Random forest is a supervised ensemble learning algorithm that is used for both classifications as well as regression problems.
- But however, it is mainly used for classification problems.
- the random forest algorithm creates decision trees on data samples and then gets the prediction from each of them and finally selects the best solution by means of voting.
- It is an ensemble method that is better than a single decision tree because it reduces the over-fitting by averaging the result.

**K nearest neighbours**

- K-Nearest Neighbour is one of the simplest Machine Learning algorithms based on Supervised Learning technique.
- K-NN algorithm assumes the similarity between the new case/data and available cases and put the new case into the category that is most similar to the available categories.
- K-NN algorithm stores all the available data and classifies a new data point based on the similarity. This means when new data appears then it can be easily classified into a well suite category by using K- NN algorithm.
- K-NN algorithm can be used for Regression as well as for Classification but mostly it is used for the Classification problems.
- K-NN is a non-parametric algorithm, which means it does not make any assumption on underlying data.
- It is also called a lazy learner algorithm because it does not learn from the training set immediately instead it stores the dataset and at the time of classification, it performs an action on the dataset.
- KNN algorithm at the training phase just stores the dataset and when it gets new data, then it classifies that data into a category that is much similar to the new data.
- Example: Suppose, we have an image of a creature that looks similar to cat and dog, but we want to know either it is a cat or dog. So for this identification, we can use the KNN algorithm, as it works on a similarity measure. Our KNN model will find the similar features of the new data set to the cats and dogs images and based on the most similar features it will put it in either cat or dog category.
