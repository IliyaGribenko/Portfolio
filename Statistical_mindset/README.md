# Understanding A/B testing through Monte Carlo simulation

**Work description**

In this paper, we discuss two samples with different conversions. Each sample consists of numbers 1 and 0 in some proportion, where 1 is the target action. 

We will conduct proportional tests. The purpose of the tests is to determine whether the samples belong to the same general population or not. 

Lets formulate the null hypothesis:

**H0: there is no difference between samples (samples belong to the same general population)**

We will conduct A/A and A/B tests with the following methods:
- Monte Carlo
- T-test
- Z-test

**Objectives of the work:**
- understand how to simulate a test of proportions using Monte Carlo
- imagine the distribution of p-values in different cases
- intuitively and logically understand the terms such as power, significance level, p-value and relationship between them

**Assumptions**

If the power or significance level of the simulated test (Monte-Carlo) differs from the expected parameters for a given sample size by more then 20 percent, then we will assume that the p-value generator is designed incorrectly.

**Stack:**
- python
- pandas
- numpy
- matplotlib
- seaborn
- statsmodels
- scipy

**Conclusion**

We did not get a big difference between the planned and the actual power, the planned and the actual alpha, from this we can conclude that we correctly conducted the simulation of the test.

I hope that for those who have viewed this notebook, the testing has become a little clearer.
