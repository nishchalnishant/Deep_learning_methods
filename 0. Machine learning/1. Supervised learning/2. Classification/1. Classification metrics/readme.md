Most of the metrics in the classification are based on the TP, FP, TN, FN

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/classification.jpeg?raw=true)

Metrics that can be used for classification techniques --

**Accuracy**

- Measures how often the classifier correctly predicts.
- High accuracy rate can be misleading , most probably we are overfitting in this case.
- Useful metric in cases where the target class is well balanced but is not good in cases of unbalanced classes

**Precision**

- Explains how many of the correctly predicted cases actually turned out to be posetive .
- Precision is useful in the cases where false posetive is higher concern than false negatives. as in cases such as music or videoo recommendation systems.

**Recall**

- Explains how many of the actual posetive cases we are able to predict correctly.
- Useful when false negative is of heigher concern than fasle posetive as in medical cases where it doesn't matter whether we raise a false alarm but the actual posetive cases should not go undetected

**F1 score**

- gives combined idea about precision and recall metrics .
- maximum when precision is equal to recall.
- punishes extreme values more , it is an effective evaluation metrics when
- false posetive and false negatives are equally costly
- adding more data doesn't effectively change the outcome
- true negative is high

**Confusion matrix**

- It is a table with combinations of predicted and actual values.

**ROC curve**

- probability curve b/w true posetive rate and false posetive rate.
- seperates signal from noise.

**Area under curve**

- measures the ability of a classifier to distinguish between clases .
- greater the area under curve the better is the performance of the model at different threshold points between posetive and negative classes .
- When AUC is equal to 1, the classifier is able to perfectly distinguish between all Positive and Negative class points. When AUC is equal to 0, the classifier would be predicting all Negatives as Positives and vice versa. When AUC is 0.5, the classifier is not able to distinguish between the Positive and Negative classes.

**log loss / logistic loss or cross entropy loss**

- the complete formula can be divided into --
- When the actual class is 1: second term in the formula would be 0 and we will left with first term i.e. yi.log(p(yi)) and (1-1).log(1-p(yi) this will be 0.

- When the actual class is 0: First-term would be 0 and will be left with the second term i.e (1-yi).log(1-p(yi)) and 0.log(p(yi)) will be 0.
