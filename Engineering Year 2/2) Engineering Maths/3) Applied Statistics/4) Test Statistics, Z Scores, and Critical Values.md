How can we use what we've learned?
One potential use of statistics is checking manufacturer claims:
>An electronics manufacturer claims that their resistor production line produces 1 kOhm resistors with a standard deviation of 50 Ohms (assume normally distributed) A process control engineer takes a sample of 5 resistors from the production line and measures the mean resistance as 1030 Ohms Is the production line working as expected?

Since we're assume that the observations $X$ are normally distributed, we know that the sample mean $\bar{X}$ will also be normally distributed (and therefore the Central Limit Theorem doesn't apply):
Therefore we have:
$$X\sim N(\mu,\sigma^{2})=N(1000,50^{2})$$
We have taken 5 observations, therefore:
$$\bar{X}\sim N(\mu,\sigma^{2}/n)=N(1000,50^{2}/5)$$
At this point we could calculate the p-value after deciding on the null hypothesis.
**Our base case would be the average resistance is 1 kilo-ohm**
**With the alternate hypothesis being: the average resistance is not 1 kilo-ohm (a two tailed test as we are very close to the true resistance.)**
### Test Statistics
p-values require the calculating of probabilities, but we can be lazy...
Instead we can use the values of $P(\bar{X}\ge 1030)$ and $P(\bar{X}\le 1030)$.. If we transform the sample mean to follow a standard normal distribution:
$$Z=\frac{\bar{X}-\mu}{\sigma/\sqrt{n}}=\frac{1030-1000}{50/\sqrt{5}}=1.34$$
This is the "Z Score" and it is an example of a **test statistic**.
### Critical Values
Instead of calculating the probability of an observation (or something more extreme) find the value of the observation (Z Score) at which the significance level is achieved.
From the probability tables for normal distributions, e.g. $P(Z\le 1.96)=0.975$:
![[Pasted image 20250410151137.png|centre]]
To test the null hypothesis we compare the Z score against the critical value. 
So for a one tailed test at a 5% significance level, don't reject $H_{0}$ if:
$$Z\le1.645~~\text{(Right-Tailed)~or~}Z\ge-1.645~~\text{Left-Tailed}$$
For a two-tailed test at 5% significance, don't reject $H_{0}$ if:
$$-1.96\le Z\le1.96$$
