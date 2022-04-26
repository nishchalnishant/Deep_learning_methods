# About --

- SVM tries to find a line/hyperplane (in multidimensional space) that separates these two classes. Then it classifies the new point depending on whether it lies on the positive or negative side of the hyperplane depending on the classes to predict.

- Our best fit line is the hyperplane that has a maximum number of points.

- The first thing that we’ll understand is what is the decision boundary which is say 'a' distance from the hyperplane. Thus, lines are at +a and -a distance from the hyperplane.

- We can find the equation of the descision boundary using the equation of the hyperplane, as it is at +a and -a distance from the hyperplane.

- Our main aim here is to decide a decision boundary at ‘a’ distance from the original hyperplane such that data points closest to the hyperplane or the support vectors are within that boundary line.

-

# Terms related to the SVM algorithm

- Kernel - helps us find a hyperplane in the higher dimensional space without increasing the computational cost. Usually, the computational cost will increase if the dimension of the data increases. This increase in dimension is required when we are unable to find a separating hyperplane in a given dimension and are required to move in a higher dimension.

- Hyperplane: This is basically a separating line between two data classes in SVM. But in Support Vector Regression, this is the line that will be used to predict the continuous output.

- Decision Boundary: A decision boundary can be thought of as a demarcation line (for simplification) on one side of which lie positive examples and on the other side lie the negative examples. On this very line, the examples may be classified as either positive or negative. This same concept of SVM will be applied in Support Vector Regression as well

**Pros:**

- Works really well on high dimensional data.
- Memory efficient.
- Effective in cases where the number of dimensions is greater than the number of samples.

**Cons:**

- Not suitable for large datasets.
- Doesn’t work well when the dataset has noise, i.e., the target classes are overlapping.
- Slow to train.
- No probabilistic explanation for classification.

credits:
https://www.analyticsvidhya.com/blog/2020/03/support-vector-regression-tutorial-for-machine-learning/
