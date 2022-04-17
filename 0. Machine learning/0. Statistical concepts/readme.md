# Important statistical terms used in machine learning

# Key terms for Data typs --

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

- Data that can take on only integer values , such as counts.
  **_Continous Data_**

- Data that can take on any value in an interval.

**_Categorical data_**

- Data taht can take on only a specific set of values representing a set of possible categories .
- Ex- Gender

**_Binary_**

- A special case of categorical data with just two categories of values[True/False].

# KEY TERMS FOR RECTANGULAR DATA

**Data frame**

- Rectangular data (like a spreadsheet) is the basic data structure for statistical and machine learning models.

**Feature**

- A column in the table is commonly referred to as a feature.

# Measures of central tendency --

**Mean**

- Also known as airthemetic mean or average.
- It can be expressed as fraction of the sum of obervations and number of observations.

**Weighted mean**

- The sum of all values times a weight divided by the sum of the weights.

**Median**

- Value seperating the upper half with the lower half of the sample or population.

**Mode** --

- Represents the most frequent observation in a numeric variable.

**Robust**

- Not sensitive to extreme values.

**Outlier**

- A data value that is very different from most of the data.

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

# KEY TERMS FOR VARIABILITY METRICS

**Deviations** --

- The difference between the observed values and the estimate of location.

**Mean absolute deviation** --

- absolute deviation from the mean
- describes the variation in the data set.

**Median absolute deviation from the median**

- The median of the absolute value of the deviations from the median.

**Variance** --

- Measure how far is data point is from the mean, only the difference from MAD and variance is we take square here.
- Variance is computed by finding the difference between each data point and mean, squaring them, summing them up, and take the average of all those numbers.

**Standard deviation** --

- The standard deviation is simply the square root of variance so we get again the value in the same measurement.
- Also measures dispersion around the mean but in the same unit as the values.
- Sigma is used to denote std. deviation of the populations and s is used as the standard deviation of the sample.

**Median absolute deviation** --

- Median of all the numbers obtained from subtracting and calculating the absolute value of every observation with the median.

# KEY TERMS FOR EXPLORING THE DISTRIBUTION --

**Boxplot**

- A plot introduced by Tukey as a quick way to visualize the distribution of data.

**Frequency table**

- A tally of the count of numeric data values that fall into a set of intervals (bins).

**Histogram**

- A plot of the frequency table with the bins on the x-axis and the count (or proportion) on the y-axis.

**Density plot**
A smoothed version of the histogram, often based on a kernal density estimate.

# Data and Sampling Distributions --

**Population**

- Entire group one desires information about.
- Ex -- population studying the voters in an election.

**Sample**

- Subset of the population taken when entire population is too large to tanalyze its charachteristics.
- Ex -- first time voters in an election.

**Random sampling**

- Drawing elements into a sample at random.

**Stratified sampling**

- Dividing the population into strata and randomly sampling from each strata.

**Simple random sample**

- The sample that results from random sampling without stratifying the population.

**Sample bias**

- A sample that misrepresents the population.

**Central Limit Theorem**

- It says that the means drawn from multiple samples will resemble the familiar bell-shaped normal curve (see “Normal Distribution”), even if the source population is not normally distributed, provided that the sample size is large enough and the departure of the data from normality is not too great.
- allows normal-approximation formulas like the t-distribution to be used in calculating sampling distributions for inference—that is, confidence intervals and hypothesis tests.

**Standard Error**

- The standard error is a single metric that sums up the variability in the sampling distribution for a statistic.
- The standard error can be estimated using a statistic based on the standard deviation s of the sample values, and the sample size n

**Bootstrap sample**

- A sample taken with replacement from an observed data set.

**Resampling**

- The process of taking repeated samples from observed data; includes both bootstrap and permutation (shuffling) procedures.

**Confidence level**

- The percentage of confidence intervals, constructed in the same way from the same population, expected to contain the statistic of interest.

**Interval endpoints**

- The top and bottom of the confidence interval.

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

**Skewness** --

- Measure of the symmetry of distribution that you plot in form of a histogram.
- A distribution is symmetrical when the proportion of data at an equal distance from the mean (or median) is equal.
- If the values extend to the right, it is right-skewed, and if the values extend left, it is left-skewed.

**Kurtosis** -

- Kurtosis in statistics is used to check whether the tails of a given distribution have extreme values.
- It also represents the shape of a probability distribution.

# Distributions

**Normal distribution** --

- Distribution in form of a bell curve and most of the datasets in machine learning follow a normal distribution and if not then we try to transform it into normal distribution and many machine learning algorithms work very well on this distribution .
- In a normal distribution , 68% of the data lies within one standad deviation of the mean, and 95% lies within two standard deviations.
- A standard normal distribution is one in which the units on the x-axis are expressed in terms of standard deviations away from the mean. To compare data to a standard normal distribution, you subtract the mean then divide by the standard deviation; this is also called normalization or standardization.
- A QQ-Plot is used to visually determine how close a sample is to the normal distribution. The QQ-Plot orders the z-scores from low to high, and plots each value’s z-score on the y-axis; the x-axis is the corresponding quantile of a normal distribution for that value’s rank. Since the data is normalized, the units correspond to the number of standard deviations away of the data from the mean.

**Long-Tailed Distributions**

- data is generally not normallydistributed.
- Sometimes, the distribution is highly skewed , the tails of a distribution correspond to the extreme values (small and large). Long tails, and guarding against them, are widely recognized in practical work.

**t-Distribution**

- t-distribution is a normally shaped distribution, but a bit thicker and longer on the tails. It is used extensively in depicting distributions of sample statistics.
- Distributions of sample means are typically shaped like a t-distribution.
- The t-distribution is actually a family of distributions resembling the normal distribution, but with thicker tails.
- It is widely used as a reference basis for the distribution of sample means, differerences between two sample means, regression parameters, and more.

**Binomial Distribution**

- The binomial distribution is the frequency distribution of the number of successes (x) in a given number of trials (n) with specified probability (p) of success in each trial.
- There is a family of binomial distributions, depending on the values of x, n, and p.
- Binomial outcomes are important to model, since they represent, among other things, fundamental decisions (buy or don’t buy, click or don’t click, survive or die, etc.).
- mean of a binomial distribution is n\*p ; you can also think of this as the expected number of successes in n trials, for success probability = p.
- The variance is n\*p(1-p). With a large enough number of trials (particularly when p is close to 0.50), the binomial distribution is virtually indistinguishable from the normal distribution.
- A binomial trial is an experiment with two possible outcomes: one with probability p and the other with probability 1 – p.
- With large n, and provided p is not too close to 0 or 1, the binomial distribution can be approximated by the normal distribution.

# Poisson and Related Distributions

**Lambda**

- The rate (per unit of time or space) at which events occur.

**Poisson distribution**

- The frequency distribution of the number of events in sampled units of time or space.
- Poisson distribution tells us the distribution of events per unit of time or space when we sample many such units.
- It is useful when addressing queuing questions like “How much capacity do we need to be 95% sure of fully processing the internet traffic that arrives on a server in any 5- second period?
- key parameter in a Poisson distribution is lambda. This is the mean number of events that occurs in a specified interval of time or space.
- The variance for a Poisson distribution is also lambda.
- The Poisson distribution is used to describe discrete quantitative data such as counts in which the population size n is large, the probability of an individual event is small, but the expected number of events, n, is moderate (say five or more).
- Typical examples are the number of deaths in a town from a particular disease per day, or the number of admissions to a particular hospital.
- Poisson distribution considers following assumptions;

The success probability for a short span is equal to success probability for a long period of time.

The success probability in a duration equals to zero as the duration becomes smaller.

A successful event can’t impact the result of another successful event

**Exponential distribution**

- The frequency distribution of the time or distance from one event to the next event.
- Using the same parameter that we used in the Poisson distribution, we can also model the distribution of the time between events: time between visits to a website or between cars arriving at a toll plaza.
- It is also used in engineering to model time to failure, and in process management to model,

**Weibull distribution**

- A generalized version of the exponential, in which the event rate is allowed to shift over time.
- If the event rate changes over the time of the interval, the exponential (or Poisson) distributions are no longer useful. This is likely to be the case in mechanical failure—the risk of failure increases as time goes by. The Weibull distribution is an extension of the exponential distribution, in which the event rate is allowed to change, as specified by a shape parameter, beta. If beta > 1, the probability of an event increases over time, if beta < 1, it decreases.
- Because the Weibull distribution is used with time-to-failure analysis instead of event rate, the second parameter is expressed in terms of characteristic life, rather than in terms of the rate of events per interval. The symbol used is , the Greek letter eta. It is also called the scale parameter.

**Bernoulli**

- - Bernoulli distribution has only two possible outcomes, namely 1 (success) and 0 (failure), and a single trial.
- - So the random variable X which has a Bernoulli distribution can take value 1 with the probability of success, say p, and the value 0 with the probability of failure, say q or 1-p.

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

# Statistical Experiments and Significance Testing

**A/B Testing**

- A/B test is an experiment with two groups to establish which of two treatments, products, procedures, or the like is superior.
- A/B tests are common in web design and marketing, since results are so readily measured.
- Some examples of A/B testing include:
  Testing two soil treatments to determine which produces better seedgermination
  Testing two therapies to determine which suppresses cancer more effectively

**Hypothesis testing**

- Uses statistical tests to determine if a hypothesis is true.
- hypothesis test assumes that the null hypothesis is true, creates a “null model” (a probability model), and tests whether the effect you observe is a reasonable outcome of that model.
- Null hypothesis (H_0) -- is the statement that there is no statistically significant difference or relationship between variables. A null hypothesis is a logical construct embodying the notion that nothing
  special has happened, and any effect you observe is due to random chance.
- Alternate hypothesis (H_1) -- is the statement created by researchers when they speculate upon the outcome of a research or experiment. It states that there is a statistically significant difference or relationship between variables.
- One-way test -- Hypothesis test that counts chance results only in one direction.
- Two-way test -- Hypothesis test that counts chance results in two directions
- Example:
  H0: The average BMI of boys and girls in a class is the same

  H1: The average BMI of boys and girls in a class is not the same

- To determine whether a finding is statistically significant, you need to interpret the p-value.
- It is common to compare the p-value to a threshold value called the significance level.

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

**ANOVA**

**Chi-Square test**

**Concetps**

- Bias -- wrong assumptions when training -> can't capture unerlying patterns -> BHU-- high bias underfit
- Varriance -- sensetive to fluctuations when training -> can't generalize on unseen data -> Overfit
- Bias varriance tradeoff -- attempts to minimize these two sources of error , through methods such as :
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - cross validation to generalize to unseen data
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; - Dimension reduction and feature selection
- Type 1 error -- Mistakenly concluding an effect is real (when it is due to chance).
- Type 2 error -- Mistakenly concluding an effect is due to chance (when it is real).
