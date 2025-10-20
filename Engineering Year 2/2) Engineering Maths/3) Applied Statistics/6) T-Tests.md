>A particular brewery is concerned about the quality control of their stouts; the aim is to produce drinks with 5.5% alcohol by volume Five different batches are measured and found to have alcohol contents of: 
>5.3, 4.3, 5.0, 4.9, 5.4 
>Assuming normality, to 5% significance (statistical power?) is there a problem with quality control?
>(Null hypothesis?)

So far we've assumed we know all the parameters of the null distribution.
**Population mean** is usually part of the null hypothesis - usually testing the hypothesised population mean against the sample mean.
**Population variance** is unknown in this question.
### Sample Variance
We can replace population variance with an estimate using sample variance:
$$s^{2}=\frac{1}{n-1}\sum\limits_{i=1}^{n}(X_{i}-\bar{X})^{2}$$
This estimate is:
**Consistent** - as $n\rightarrow\infty$ we have $s^{2}\rightarrow\sigma^{2}$ in probability so with enough data it will produce an accurate result
**Unbiased** - the expected value $E[s^{2}]=\sigma^{2}$ so on average it doesn't under or over predict the result.

Sample space variance $S^{2}$ is a random variable with:
$$(n-1)\frac{s^{2}}{\sigma^{2}}\sim X_{n-1}^{2}$$
Where:
- $n$ is the number of observations
- $X_{n-1}^{2}$ is the chi-squared distribution with $n-1$ degrees of freedom
### T Scores
Instead of using a Z score we now use a T Score
$$T=\frac{\bar{X}-\mu}{s/\sqrt{n}}$$
As before $\bar{X}$ is normally distributed but now $s$ is a random variable as well.
$T$ follows Student's T-Distribution with $n-1$ degrees of freedom.
We need to use the **corresponding critical values** instead of those from the normal distribution.
### Student's T-Distribution
![[Pasted image 20250410155531.png|centre]]
### Statistical Insignificance for Low DOF
![[Pasted image 20250410155600.png|centre]]
So with low DOF the critical values are so high that there is no statistical significance.

>With the data provided $\bar{X}$ = 4.98, $s^2$ = 0.187 and $s$= 0.432 If this were a Z score† (normally distributed), would you reject the null hypothesis at 5% significance? 
>(† This is a hypothetical question — it’s not a Z score!)

Going back to the original question:
With the data provided:
- $\bar{X}=4.98$
- $s^2=0.187$
- $s=0.432$
So:
$$T=\frac{\bar{X}-\mu}{s/\sqrt{n}}=\frac{4.98-5.5}{0.432/\sqrt{5}}=-2.689$$
At $n-1=4$ degrees of freedom, the critical value for a two-tailed T test is $\pm 2.776$ and therefore **we cannot reject the null hypothesis.**
