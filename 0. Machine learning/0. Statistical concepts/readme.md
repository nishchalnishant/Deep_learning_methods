# Important statistical terms used in machine learning

**Population**

- Entire group one desires information about.

**Sample**

- Subset of the population taken when entire population is too large to tanalyze its charachteristics

# Measures of central tendency --

**Mean**

- Also known as airthemetic mean or average.
- It can be expressed as fraction of the sum of obervations and number of observations.

**Median**

- Value seperating the upper half with the lower half of the sample/population.

**Mode** --

- Represents the most frequent observation in a numeric variable.

# Measures of spread --

**Range** --

- difference between the largest and smallest point in your data (max-min).

**Percentiles** --

- measure used in statistics indicating the value below which a given percentage of observation in a group of observations falls. for example, the 20th percentile is a value below which 20 per cent of data falls.

**Quartiles** --

- values that divide a list of numbers into quarters. the steps to find the quartile is.

- Put the list of numbers in order
- Then cut the list into 4 equal parts
- The quartiles are at the cuts

**Interquartile range** --

- measure of dispersion between upper(75th) and lower(25th) Quartiles. It is a very important term in statistics that is used in most calculations and data preprocessing like dealing with outliers.

**Mean absolute deviation** --

- absolute deviation from the mean
- describes the variation in the data set.

**Variance** --

- measure how far is data point is from the mean, only the difference from MAD and variance is we take square here.
- variance is computed by finding the difference between each data point and mean, squaring them, summing them up, and take the average of all those numbers.

**Standard deviation** --

- the standard deviation is simply the square root of variance so we get again the value in the same measurement.
- also measures dispersion around the mean but in the same unit as the values.
- sigma is used to denote std. deviation of the populations and s is used as the standard deviation of the sample.

**Median absolute deviation** --

- Median of all the numbers obtained from subtracting and calculating the absolute value of every observation with the median.

**Normal distribution** --

- Distribution in form of a bell curve and most of the datasets in machine learning follow a normal distribution and if not then we try to transform it into normal distribution and many machine learning algorithms work very well on this distribution .

**Skewness** --

- measure of the symmetry of distribution that you plot in form of a histogram.

**Central limit theorm**
**Probability density function**
**cumulative distributive function**
**Hypothesis testing**

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

| Test Method | Compare                                          | Result                            |
| ----------- | ------------------------------------------------ | --------------------------------- |
| Classical   | test statistic > critical value(i.e. F > F crit) | Reject the null hypothesis        |
| Classical   | test statistic < critical value(i.e. F < F crit) | Cannot reject the null hypothesis |
| p value     | p value < α                                      | Reject the null hypothesis        |
| p value     | p value > α                                      | Cannot reject the null hypothesis |

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
