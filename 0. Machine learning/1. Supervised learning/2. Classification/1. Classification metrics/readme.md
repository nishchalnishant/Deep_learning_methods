Most of the metrics in the classification are based on the TP, FP, TN, FN

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/classification.jpeg?raw=true)

Metrics that can be used for classification techniques --

**Accuracy**
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
  false posetive and false negatives are equally costly
  adding more data doesn't effectively change the outcome
  true negative is high

**Confusion matrix**

**ROC curve**

- probability curve b/w true posetive rate and false posetive rate.
- seperates signal from noise.

**Area under curve**

- measures the ability of a classifier to distinguish between clases .
- greater the area under curve the better is the performance of the model at different threshold points between posetive and negative classes .
- When AUC is equal to 1, the classifier is able to perfectly distinguish between all Positive and Negative class points. When AUC is equal to 0, the classifier would be predicting all Negatives as Positives and vice versa. When AUC is 0.5, the classifier is not able to distinguish between the Positive and Negative classes.

**log loss / logistic loss or cross entropy loss**
