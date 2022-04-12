**Use cases**

- Image classification
- Customer retention
- Identity fraud detection
- Diagnostics

# Metrics that can be used for classification techniques --

**Accuracy**

- (TP+TN)/(TP+TN+FP+FN)
- Ratio of number of correct predictions to the total number of predictions.

**Precision**

- (TP)/(TP+FP)

**Recall/Sensitivity**

- TP/(TP+FN)

**F1 score**

- harmonic mean of precision and recall
- 2*(precision*recall)/(precision+recall)

**Confusion matrix**
**ROC curve**
probability curve b/w true posetive rate and false posetive rate.
seperates signal from noise.

- Area under curve -
  in Roc curve the X-axis value shows False Positive Rate (FPR), and Y-axis shows True Positive Rate (TPR). Higher the value of X means higher the number of False Positives(FP) than True Negatives(TN), while a higher Y-axis value indicates a higher number of TP than FN. So, the choice of the threshold depends on the ability to balance between FP and FN.
- log loss / logistic loss or cross entropy loss
  logloss= -1/N*(y*log(p)+(1-y)\*log(1-p))

# Algorithms for classification

**Logistic regression**

- similar to linear regression but is used to model the probability of a discrete number of outcomes
- First, we calculate a score using an equation similar to the equation for the line of best fit for linear regression.
- The extra step is feeding the score that you previously calculated in the sigmoid function below so that you get a probability in return. This probability can then be converted to a binary output, either 1 or 0.
- To find the weights of the initial equation and calculate the score, methods like gradient descent or maximum likelihood are used.

- Random forest
- Naive bayes
- Support vector machines
- Descision tree
- Gradient boosted tree
- XGBoost
- LightGBM
- CatBoost
