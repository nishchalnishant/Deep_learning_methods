## ABOUT --

- Naive bayes model is easy to build and is mostly used for large datasets
- It is called Naive because of the assumption that 2 variables are independent when they may not be. In a real-world scenario, there is hardly any situation where the features are independent.
- We use Bayes theorm for Bayes algorithm.

## Applications of Naive Bayes Algorithms

**_Real time Prediction_**:

- Naive Bayes is an eager learning classifier and it is sure fast. Thus, it could be used for making predictions in real time.

**_Multi class Prediction_**: This algorithm is also well known for multi class prediction feature. Here we can predict the probability of multiple classes of target variable.

**_Text classification/ Spam Filtering/ Sentiment Analysis_**: Naive Bayes classifiers mostly used in text classification (due to better result in multi class problems and independence rule) have higher success rate as compared to other algorithms. As a result, it is widely used in Spam filtering (identify spam e-mail) and Sentiment Analysis (in social media analysis, to identify positive and negative customer sentiments)

**_Recommendation System_**: Naive Bayes Classifier and Collaborative Filtering together builds a Recommendation System that uses machine learning and data mining techniques to filter unseen information and predict whether a user would like a given resource or not

**Pros:**

- Gives high performance when the conditional independence assumption is satisfied.
- Easy to implement because only probabilities need to be calculated.
- Works well with high-dimensional data, such as text.
- Fast for real-time predictions.

**Cons:**

- If conditional independence does not hold, then is performs poorly.
- Has the problem of Numerical Stability or Numerical Underflow because of the multiplication of several small digits.
