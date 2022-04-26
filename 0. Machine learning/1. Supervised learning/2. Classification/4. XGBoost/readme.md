# ABOUT--

-The beauty of this powerful algorithm lies in its scalability, which drives fast learning through parallel and distributed computing and offers efficient memory usage.

- XGBoost is an ensemble learning method.

- Ensemble learning offers a systematic solution to combine the predictive power of multiple learners.

- The models that form the ensemble, also known as base learners, could be either from the same learning algorithm or different learning algorithms.

- Bagging and boosting are two widely used ensemble learners.

> **_Bagging_**

- While decision trees are one of the most easily interpretable models, they exhibit highly variable behavior.
- If we consider a single training dataset that we randomly split into two parts.
- Now, we can use each part to train a decision tree in order to obtain two models.
- When we fit both these models, they would yield different results.
- Decision trees are said to be associated with high variance due to this behavior.
- Bagging or boosting aggregation helps to reduce the variance in any learner.
- Several decision trees which are generated in parallel, form the base learners of bagging technique.
- Data sampled with replacement is fed to these learners for training.
- The final prediction is the averaged output from all the learners.

> **_Boosting_**

- In boosting, the trees are built sequentially such that each subsequent tree aims to reduce the errors of the previous tree.
- Each tree learns from its predecessors and updates the residual errors.
- Hence, the tree that grows next in the sequence will learn from an updated version of the residuals.
- The base learners in boosting are weak learners in which the bias is high, and the predictive power is just a tad better than random guessing.
- Each of these weak learners contributes some vital information for prediction, enabling the boosting technique to produce a strong learner by effectively combining these weak learners.
- The final strong learner brings down both the bias and the variance.
- In contrast to bagging techniques like Random Forest, in which trees are grown to their maximum extent, boosting makes use of trees with fewer splits.
- Such small trees, which are not very deep, are highly interpretable.
- Parameters like the number of trees or iterations, the rate at which the gradient boosting learns, and the depth of the tree, could be optimally selected through validation techniques like k-fold cross validation.
- Having a large number of trees might lead to overfitting.

**_The boosting ensemble technique consists of three simple steps:_**

- An initial model F0 is defined to predict the target variable y. This model will be associated with a residual (y – F0)

- A new model h1 is fit to the residuals from the previous step

- Now, F0 and h1 are combined to give F1, the boosted version of F0. The mean squared error from F1 will be lower than that from F0:

To improve the performance of F1, we could model after the residuals of F1 and create a new model F2:

This can be done for ‘m’ iterations, until residuals have been minimized as much as possible:

Here, the additive learners do not disturb the functions created in the previous steps. Instead, they impart information of their own to bring down the errors.

- **Pros:**

- Can work in parallell.
- Can handle missing values.
- No need for scaling or normalizing data.
- Fast to interpret.
  Great execution speed.

**Cons:**

- Can easily overfit if parameters are not tuned properly.
- Hard to tune.
