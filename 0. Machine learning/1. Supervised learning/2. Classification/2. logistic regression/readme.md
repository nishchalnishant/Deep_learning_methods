## ABOUT

- Logistic Regression is a “Supervised machine learning” algorithm that can be used to model the probability of a certain class or event.

- It is used when the data is linearly separable and the outcome is binary or dichotomous in nature.

- In case of linear regression we fitted a straight line while in case of logistic regression we have to squeeze that line between 0 and 1 , we do that using the sigmoid function .

- we pass the rhs of the linear regression to the sigmoid activation , which forces the ouptu to assume values between 0 and 1.

- Taking logs on both sides we get log odds or logits on the LHS and on RHS the RHS of activation function.

- Now we need to find the values for the RHS to find the final equation.

**Pros**

- Easy to interpret, implement and train. Doesn’t require too much computational power.
- Makes no assumption of the class distribution.
- Fast in classifying unknown records.
- Can easily accommodate new data points.
- Is very efficient when features are linearly separable.

**Cons:**

- Tries to predict precise probabilistic outcomes, which leads to overfitting in high dimensions.
- Since it has a linear decision surface, it can’t solve non-linear problems.
- Tough to obtain complex relations other than linear relations.
- Requires very little or no multicollinearity.
- Needs a large dataset and sufficient training examples for all the categories to make correct predictions.

https://christophm.github.io/interpretable-ml-book/logistic.html

https://towardsdatascience.com/logistic-regression-detailed-overview-46c4da4303bc
