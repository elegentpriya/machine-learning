# Machine-learning
# 1. Hypothesis Testing 1: Working Mothers' Talk Time (Z-test)
Import the scipy.stats module, which provides statistical functions and distributions.

Define the given values:

sample_mean: The calculated mean from the sample data.
population_stddev: The standard deviation of the population.
sample_size: The size of the sample.
alpha: The significance level for the test.
Define the hypothesized population mean (hypothesized_mean), which is the value you want to test against.

Calculate the z-test statistic using the formula: (sample_mean - hypothesized_mean) / (population_stddev / (sample_size ** 0.5)). This statistic measures how many standard deviations the sample mean is away from the hypothesized mean.

Calculate the critical z-value using the inverse cumulative distribution function (ppf) of the standard normal distribution (stats.norm.ppf(1 - alpha)). This gives you the z-value beyond which you would reject the null hypothesis.

Compare the calculated z-test statistic with the critical z-value. If the calculated z-test statistic is greater than the critical z-value, you would reject the null hypothesis; otherwise, it fails to reject it.

# Hypothesis Testing 2: Coffee Shop Wait Time (T-test)
Import the scipy.stats module, just like in the previous example.

Define the given values, including sample_mean, sample_stddev, sample_size, and alpha.

Define the hypothesized population mean (hypothesized_mean).

Calculate the t-test statistic using the formula: (sample_mean - hypothesized_mean) / (sample_stddev / (sample_size ** 0.5)). This statistic is similar to the z-test statistic but is adapted for smaller sample sizes using the t-distribution.

Calculate the degrees of freedom (degrees_of_freedom) for the t-distribution. It's one less than the sample size.

Calculate the critical t-value using the inverse cumulative distribution function (ppf) of the t-distribution (stats.t.ppf(1 - alpha, df=degrees_of_freedom)).

Compare the calculated t-test statistic with the critical t-value. If the calculated t-test statistic is less than the critical t-value, you would reject the null hypothesis; otherwise, you would fail to reject it.
