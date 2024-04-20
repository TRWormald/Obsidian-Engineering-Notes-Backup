## Continuous Probability Distributions
Sometimes we want to map the probability of **continuous events** (where the sample space is continuous - and doesn't take discrete values).
The probability in these cases will always be an inequality as the probability of something being exactly a single value is zero (for example no-one is exactly 2m tall).
### The Normal Distribution
The normal distribution is a very common probability distribution that turns up literally everywhere. It is defined by the [[Mean and Standard Deviation]] of the data and is characterised by the fact that the mean median and mode all fall at the same value:
![[Pasted image 20240420151236.png|center|400]]
The distribution is symmetric (so 50% of data is below the mean and 50% is greater than the mean) and specific amounts of the data lies within 1, 2, and 3 standard deviations of the mean:
![[Pasted image 20240420151526.png|center|400]]
![[Pasted image 20240420151546.png|center|400]]
![[Pasted image 20240420151601.png|center|400]]
The equation for the normal distribution is:
$$f_{X}(x)=\frac{1}{\sigma\sqrt{2\pi}}e^{- \frac{1}{2\sigma^{2}}(x-\mu)^{2}}$$
Where $f_X(x)$ is the **probability density function** of the normal distribution.
\
When we define our normal distribution we do it in the following way:
$$X\sim N(\mu,\sigma^{2})$$
Where $\mu$ is the mean $\sigma^{2}$ is the variance (and $\sigma$ is the standard deviation).
#### Example of finding the probability:
Take the normal distribution:
$$X\sim N(75,8.7^{2})$$
And say we want to find $P(X>75)$:
$$P(X>75)=\int^{\infty}_{75}f_{X}(x)\cdot dx$$
This integral produces the **cumulative distribution function**:
$$\text {Cumulative Distribution Function}=\int\text{Probability density function}$$
However the integral for the normal distribution is impossible to do using standard methods so instead we use software or tables of values to evaluate the **CDF**.
### The Standard Normal Distribution
The standard normal is a normal distribution wi
## Discrete Probability Distributions
