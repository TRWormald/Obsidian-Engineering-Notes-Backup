What are the problems with small samples?
So far we have made the following underlying assumptions:
- Observations are independent
- Observations are normally distributed, or
- Enough observations have been made to assume the central limit theorem works
	- So we can assume the sample mean is normally distributed
	- T-Distribution for the sample mean also requires normally distributed observations
**These are strong assumptions**.

If we want to relax the assumption of normality or a large sample, we can turn to resampling methods.
They are a more modern approach to statistics but they cant be done by hand.
The fundamental idea is that:
1) The data you've already collected is the best representation of the distribution
2) Recombine the data you've already got to generate a distribution for hypothesis testing.
#### The Difference of Two Sample Means
Lets have two samples: the length of hospital stay for two groups - one given a new treatment, and a control.
![[Pasted image 20250411200838.png|centre]]
The difference is -5.4 but the two samples are too small for the CLT to apply (so we cannot use a difference of two sample means t-test)
Our Null Hypothesis is that the treatment does nothing.
The implication is that both samples are drawn from the same population.

Since samples are assumed to be from the same population we can reshuffle the groups without affecting the distribution.

There are $\left(\begin{matrix}10\\5\end{matrix}\right)=252$ different ways of grouping the 10 observations into two groups.
For each shuffled combination, calculate the difference between the sample means.
Use all these combinations to generate a sampling distribution.
![[Pasted image 20250411201141.png|centre]]
We can repeat this many times and we can then generate a histogram:
![[Pasted image 20250411201227.png|centre]]
We can then get an estimate of the p-value from the number of calculated values above/below the observed value.
![[Pasted image 20250411201316.png|centre]]
Therefore we reject the null hypothesis as it's less than our significance level of 5%.
This works for comparing two samples, but what about a single sample, then we need to use the **bootstrap method**.
### The Bootstrap Method
![[Pasted image 20250411201448.png|centre]]
![[Pasted image 20250411201500.png|centre]]
Again we repeat many times and generate a histogram:
![[Pasted image 20250411201523.png|centre]]
Bootstrap can be used for many different types of statistic, not just the mean.
It is **asymptotically accurate**:
- Requires a large number of observations in the original sample to produce accurate results
- But works reasonable for small numbers of observations
- And you often don't have any other choices for small samples
It can be easily implemented in many programming languages.