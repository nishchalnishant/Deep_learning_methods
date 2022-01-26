# Important statistical terms used in machine learning

**Population**

- Entire group one desires information about.

**Sample**

- Subset of the population taken when entire population is too large to tanalyze its charachteristics

**Mean**

- Also known as airthemetic mean or average.
- It can be expressed as fraction of the sum of obervations and number of observations.

**Median**

- Value seperating the upper half with the lower half of the sample/population.

**Variance**

- Measures dispersion around the mean.
- Determined by averaging the squared differences of all the values from the mean.
- can be calculated by substracting the square of the mean from the average of squared scores.

**Standard deviation**

- Squared root of the varriance
- also measures dispersion around the mean but in the same unit as the values.
- sigma is used to denote std. deviation of the populations and s is used as the standard deviation of the sample.

**Standard error**

- An estimate of the standard deviation of the sampaling distribution the set of all the samples of size n that can be taken from a population.
- Reflects the extent to which a statistic changes from sample to sample.

**Hypothesis testing**

- Uses statistical tests to determine if a hypothesis is true
- Null hypothesis (H_0) -- is the statement that there is no statistically significant difference or relationship between variables.
- Alternate hypothesis (H_1) -- is the statement created by researchers when they speculate upon the outcome of a research or experiment. It states that there is a statistically significant difference or relationship between variables.

Three Hypothesis testing methods --

- Classical -- compare a test statistics to a critical value.
- P value -- Probability of a test statistics being contrary to the null hypothesis.
- Confidence interval -- Test statistics between or outside of the confidence interval

Error --

- Type 1 -- Reject a null hypothesis that is true
- Type 2 -- Not reject a null hypothesis that is false.

**Interpreting the Results**
|Test Method |Compare |Result|
|------------|--------|------|
|Classical |test statistic > critical value
(i.e. F > F crit) |
Reject the null hypothesis|
|Classical |test statistic < critical value
(i.e. F < F crit) |
Cannot reject the null hypothesis|
|p value |p value < α |Reject the null hypothesis|
|p value |p value > α |Cannot reject the null
hypothesis|

**T-test**

- **_Distributions_**

- it can be descrete as well as continous

**Binomial**

- Binomail
- Geometric
- Negative binomial
- Hypergeometric
- Poisson

**contibous**

- Uniform
- Normal/Gaussian
- Exponential
- Gamma

**Concetps**

- Bias -- wrong assumptions when training -> can't capture unerlying patterns -> BHU-- high bias underfit
- Varriance -- sensetive to fluctuations when training -> can't generalize on unseen data -> Overfit
- Bias varriance tradeoff -- attempts to minimize these two sources of error , through methods such as :
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - cross validation to generalize to unseen data
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Dimension reduction and feature selection
