Most of the metrics in the classification are based on the TP, FP, TN, FN

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/classification.jpeg?raw=true)

Metrics that can be used for classification techniques --

**Accuracy**

- Measures how often the classifier correctly predicts.
- High accuracy rate can be misleading , most probably we are overfitting in this case.
- Useful metric in cases where the target class is well balanced but is not good in cases of unbalanced classes.

> When to use it:

- When your problem is balanced using accuracy is usually a good start.
- An additional benefit is that it is really easy to explain it to non-technical stakeholders in your project,
- When every class is equally important to you.

**Precision**

- Explains how many of the correctly predicted cases actually turned out to be posetive .
- Precision is useful in the cases where false posetive is higher concern than false negatives. as in cases such as music or videoo recommendation systems.

> When to use it:

- Again, it usually doesn’t make sense to use it alone but rather coupled with other metrics like recall.
- When raising false alerts is costly, when you want all the positive predictions to be worth looking at you should optimize for precision.

**Recall**

- Explains how many of the actual posetive cases we are able to predict correctly.
- Useful when false negative is of heigher concern than fasle posetive as in medical cases where it doesn't matter whether we raise a false alarm but the actual posetive cases should not go undetected.

> When to use it:

- Usually, you will not use it alone but rather coupled with other metrics like precision.
- That being said, recall is a go-to metric, when you really care about catching all fraudulent transactions even at a cost of false alerts.
- Potentially it is cheap for you to process those alerts and very expensive when the transaction goes unseen.

**F1 score**

- gives combined idea about precision and recall metrics .
- maximum when precision is equal to recall.
- punishes extreme values more , it is an effective evaluation metrics when
- false posetive and false negatives are equally costly
- adding more data doesn't effectively change the outcome
- true negative is high.

> When to use it:

- Pretty much in every binary classification problem. It is my go-to metric when working on those problems.
- It can be easily explained to business stakeholders.

**Confusion matrix**

- It is a table with combinations of predicted and actual values.

> When to use it:

- Pretty much always. I like to see the nominal values rather than normalized to get a feeling on how the model is doing on different, often imbalanced, classes.

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/conf_matrix.png?raw=true)

**ROC curve**

- probability curve b/w true posetive rate and false posetive rate.
- seperates signal from noise.

> When to use it:

- ROC curves are frequently used to show in a graphical way the connection/trade-off between clinical sensitivity and specificity for every possible cut-off for a test or a combination of tests.
- In addition the area under the ROC curve gives an idea about the benefit of using the test(s) in question.

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/roc_auc_curve.png?raw=true)

**Area under curve**

- measures the ability of a classifier to distinguish between clases .
- greater the area under curve the better is the performance of the model at different threshold points between posetive and negative classes .
- When AUC is equal to 1, the classifier is able to perfectly distinguish between all Positive and Negative class points. When AUC is equal to 0, the classifier would be predicting all Negatives as Positives and vice versa. When AUC is 0.5, the classifier is not able to distinguish between the Positive and Negative classes.

> When to use it:

- You should use it when you ultimately care about ranking predictions and not necessarily about outputting well-calibrated probabilities (read this article by Jason Brownlee if you want to learn about probability calibration).
- You should not use it when your data is heavily imbalanced. It was discussed extensively in this article by Takaya Saito and Marc Rehmsmeier. The intuition is the following: false positive rate for highly imbalanced datasets is pulled down due to a large number of true negatives.
- You should use it when you care equally about positive and negative classes. It naturally extends the imbalanced data discussion from the last section. If we care about true negatives as much as we care about true positives then it totally makes sense to use ROC AUC.

**log loss / logistic loss or cross entropy loss**

- the complete formula can be divided into --
- When the actual class is 1: second term in the formula would be 0 and we will left with first term i.e. yi.log(p(yi)) and (1-1).log(1-p(yi) this will be 0.

- When the actual class is 0: First-term would be 0 and will be left with the second term i.e (1-yi).log(1-p(yi)) and 0.log(p(yi)) will be 0.

> When to use it:

- Pretty much always there is a performance metric that better matches your business problem.
- Because of that, I would use log-loss as an objective for your model with some other metric to evaluate performance.

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/log_loss.png?raw=true)
