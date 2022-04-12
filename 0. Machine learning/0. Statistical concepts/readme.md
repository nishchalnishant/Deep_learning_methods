# Important statistical terms used in machine learning

**Population**

- Entire group one desires information about.
- Ex -- population studying the voters in an election.

**Sample**

- Subset of the population taken when entire population is too large to tanalyze its charachteristics.
- Ex -- first time voters in an election.

# Data typs --

**Qualitative data**

- Can't be expressed as a number and can't be measured.
- Consists of words, pictures and symbols, not numbers.
- Also known as categorical data as information can be stored by category, not by numbers.
- Ex-- colrs, names, ethinicoity.

**_Nominal Data_**

- Used just for labeling variables , without any type of quantitative values.
- Just name a thing without applying it to order , can just be called labels.
- Ex-- Gender ( Men, Women), Hair color ( Blonde , Brown etc.), Marital Status (Married, Single, Widowed)

**_Ordnial Data_**

- Showes where a number is in order .
- Data which is placed into some kind of order by their position on a scale, these may indicate superiority.

**Quantative data**

- Can be expressed as numbers ,measured by numerical variables.
- Easily amenable to statistical manipulation and can be represented by Graphs.
- Ex- Scores on test and exams, The weight of a person or a subject, Shoe size.

**_Discrete Data_**

**_Continous Data_**

# Measures of central tendency --

**Mean**

- Also known as airthemetic mean or average.
- It can be expressed as fraction of the sum of obervations and number of observations.

**Median**

- Value seperating the upper half with the lower half of the sample or population.

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

- measure of dispersion between upper(75th) and lower(25th) Quartiles.
- It is a very important term in statistics that is used in most calculations and data preprocessing like dealing with outliers.

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
- A distribution is symmetrical when the proportion of data at an equal distance from the mean (or median) is equal.
- If the values extend to the right, it is right-skewed, and if the values extend left, it is left-skewed.

**Kurtosis** -

- Kurtosis in statistics is used to check whether the tails of a given distribution have extreme values.
- It also represents the shape of a probability distribution.

**Central limit theorm**

- According to the central limit theorem, given a population with mean as μ and standard deviation as σ, if you take large random samples from the population, then the distribution of the sample means will be roughly normally distributed, irrespective of the original population distribution.

**Probability density function**

- probability density function (PDF) is used to define the random variable’s probability coming within a distinct range of values, as opposed to taking on any one value.
- The function explains the probability density function of normal distribution and how mean and deviation exists.
- defines the probability function representing the density of a continuous random variable lying between a specific range of values.
  https://byjus.com/maths/probability-density-function/

**cumulative distributive function**

- The Cumulative Distribution Function (CDF), of a real-valued random variable X, evaluated at x, is the probability function that X will take a value less than or equal to x.
- It is used to describe the probability distribution of random variables in a table

**Standard error**

- An estimate of the standard deviation of the sampaling distribution the set of all the samples of size n that can be taken from a population.
- Reflects the extent to which a statistic changes from sample to sample.

**Hypothesis testing**

- Uses statistical tests to determine if a hypothesis is true
- Null hypothesis (H_0) -- is the statement that there is no statistically significant difference or relationship between variables.
- Alternate hypothesis (H_1) -- is the statement created by researchers when they speculate upon the outcome of a research or experiment. It states that there is a statistically significant difference or relationship between variables.
- Example:
  H0: The average BMI of boys and girls in a class is the same

  H1: The average BMI of boys and girls in a class is not the same

To determine whether a finding is statistically significant, you need to interpret the p-value. It is common to compare the p-value to a threshold value called the significance level.

It often sets the level of significance to 5% or 0.05.

If the p-value > 0.05 - Accept the null hypothesis.

If the p-value < 0.05 - Reject the null hypothesis.

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

- A binomial distribution can be thought of as simply the probability of a SUCCESS or FAILURE outcome in an experiment or survey that is repeated multiple times.
- binomial distribution is closely related to the Bernoulli distribution.
- If each Bernoulli trial is independent, then the number of successes in Bernoulli trails has a binomial Distribution.
- On the other hand, the Bernoulli distribution is the Binomial distribution with n=1.”

- Bernoulli

- - Bernoulli distribution has only two possible outcomes, namely 1 (success) and 0 (failure), and a single trial.
- - So the random variable X which has a Bernoulli distribution can take value 1 with the probability of success, say p, and the value 0 with the probability of failure, say q or 1-p.

- Poisson
- - The Poisson distribution is used to describe discrete quantitative data such as counts in which the population size n is large, the probability of an individual event is small, but the expected number of events, n, is moderate (say five or more).
- - Typical examples are the number of deaths in a town from a particular disease per day, or the number of admissions to a particular hospital.
- - Poisson distribution considers following assumptions;

The success probability for a short span is equal to success probability for a long period of time.

The success probability in a duration equals to zero as the duration becomes smaller.

A successful event can’t impact the result of another successful event

**continous**

- Uniform
- - Uniform distribution can either be discrete or continuous where each event is equally likely to occur.
- - It has a constant probability constructing a rectangular distribution.
- - In this type of distribution, an unlimited number of outcomes will be possible and all the events have the same probability, similar to Bernoulli’s distribution.

- Normal/Gaussian

  - - Being a continuous distribution, the normal distribution is most commonly used in data science.
  - - A very common process of our day to day life belongs to this distribution- income distribution, average employees report, average weight of a population, etc.

- Exponential
  - - Like the poisson distribution, exponential distribution has the time element; it gives the probability of a time duration before an event takes place.
  - - Exponential distribution is used for survival analysis, for example, life of an air conditioner, expected life of a machine,and length of time between metro arrivals.
- Gamma

**Concetps**

- Bias -- wrong assumptions when training -> can't capture unerlying patterns -> BHU-- high bias underfit
- Varriance -- sensetive to fluctuations when training -> can't generalize on unseen data -> Overfit
- Bias varriance tradeoff -- attempts to minimize these two sources of error , through methods such as :
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - cross validation to generalize to unseen data
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Dimension reduction and feature selection
