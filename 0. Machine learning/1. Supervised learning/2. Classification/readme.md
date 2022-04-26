# Metrics that can be used for classification techniques --

**_Accuracy_**

- (TP+TN)/(TP+TN+FP+FN)
- Ratio of number of correct predictions to the total number of predictions.
- It measures how many observations, both positive and negative, were correctly classified.
- shouldn’t be used on an imbalanced dataset, as it is easy to get a high accuracy score by simply classifying all observations as the majority class.
- For example by classifying all transactions as non-fraudulent we can get an accuracy of over 0.9.

**_Precision_**

- (TP)/(TP+FP)
- Ratio of true posetive to sum of true posetive and false posetive.
- Also known as posetive predictive value.
- measures how many observations predicted as positive are in fact positive.

**_Recall/Sensitivity_**

- TP/(TP+FN)
- Ratio of true posetive with sum of true posetive and false negative.
- Also known as True posetive rate or sensitivity.
- measures how many observations out of all positive observations have we classified as positive.
- For example - It tells us how many fraudulent transactions we recalled from all fraudulent transactions.

**_F1 score_**

- harmonic mean of precision and recall
- 2*(precision*recall)/(precision+recall).
- Combining precision and recall gave us a more realistic view of our models.

**_Confusion matrix_**

- It is a common way of presenting true positive (tp), true negative (tn), false positive (fp) and false negative (fn) predictions.
- Those values are presented in the form of a matrix where the Y-axis shows the true classes while the X-axis shows the predicted classes.
- It is calculated on class predictions, which means the outputs from your model need to be thresholded first.

**_ROC curve_**

- Graph between True posetive rate and False posetive rate.
- probability curve b/w true posetive rate and false posetive rate.
- seperates signal from noise.
- chart that visualizes the tradeoff between true positive rate (TPR) and false positive rate (FPR).
- Basically, for every threshold, we calculate TPR and FPR and plot it on one chart.
- The higher TPR and the lower FPR is for each threshold the better and so classifiers that have curves that are more top-left side are better.

**_Area under curve_**

- In Roc curve the X-axis value shows False Positive Rate (FPR), and Y-axis shows True Positive Rate (TPR).
- Higher the value of X means higher the number of False Positives(FP) than True Negatives(TN), while a higher Y-axis value indicates a higher number of TP than FN.
- So, the choice of the threshold depends on the ability to balance between FP and FN.
- ROC AUC score is equivalent to calculating the rank correlation between predictions and targets.
- From an interpretation standpoint, it is more useful because it tells us that this metric shows how good at ranking predictions your model is.
- It tells you what is the probability that a randomly chosen positive instance is ranked higher than a randomly chosen negative instance.

**_log loss / logistic loss or cross entropy loss_**

- logloss= -1/N*(y*log(p)+(1-y)\*log(1-p))
- Log loss is often used as the objective function that is optimized under the hood of machine learning models. But, it can also be used as a performance metric.

# Algorithms for classification

**_Logistic regression_**

- Similar to linear regression but is used to model the probability of a discrete number of outcomes
- First, we calculate a score using an equation similar to the equation for the line of best fit for linear regression.
- The extra step is feeding the score that we previously calculated in the sigmoid function below so that we get a probability in return. This probability can then be converted to a binary output, either 1 or 0.
- To find the weights of the initial equation and calculate the score, methods like gradient descent or maximum likelihood are used.

> Assumption

- Target variable is binary [Can take two values].
- logistic regression does not require a linear relationship between the dependent and independent variables.
- the error terms (residuals) do not need to be normally distributed.
- requires the observations to be independent of each other.
- independent variables should not be too highly correlated with each other.
- Generally requires a larger set of exampls to train on.

**_Naive bayes_**

> Assumptions:

- The biggest and only assumption is the assumption of conditional independence.
- Support vector machines
- Descision tree
- Gradient boosted tree

**_XGBoost_**

> Assumptions --

- It may have an assumption that encoded integer value for each variable has ordinal relation.

# Apart from all above algorithms , we can also use the use random forest, support vector machine, descision tree classifier , LightGBM , CatBoostbut all these are already dsicussed in the regression tab.

**_Use cases_**

- Image classification
- Customer retention
- Identity fraud detection
- Diagnostics

**_Reference_**

> Logistic regression

- 5.2 Logistic regression: Data Science concepts and Practice ISBN: 978-0-12-814761-0
