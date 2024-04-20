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
The standard normal is a normal distribution with a mean of zero and a standard deviation of one:
$$Z\sim N(0,1)$$
It is used because it would be difficult to have a table of the CDF for each $\mu$ and $\sigma^{2}$ value - so those values are standardized to make things simpler.
This is done by subtracting the mean from every original observation and then dividing by the standard deviation.
So if you have a data point $x$ and you want to convert it to the standard normal $z$ you do:
$$z=\frac{x-\mu}{\sigma}$$
#### Example of using the Standard Normal
Taking the normal distribution below find $P(X\le 6.7)$.
$$X\sim N(4,2^{2})$$
We would first normalise:
$$Z=\frac{X-4}{2}$$
So:
$$P(X\le6.7)=P\left(Z=\frac{X-4}{2}\le \frac{6.7-4}{2}=1.35\right)=P(Z\le1.35)$$
We then put this into the table and read off the result.

### The Uniform Distribution
The uniform distribution is rather simple, the probability of any given observation is constant:
![[Pasted image 20240420161536.png|center|400]]
The probability density function is:
$$f_{X}(x)=\left\{\begin{align*}
& \frac{1}{u-l} \text{ if } l<x<u\\
& 0 \text{ otherwise}
\end{align*}\right.$$
And the cumulative distribution function is:
$$F(x)=\left\{\begin{align*}
& 0, \text{ if } x<l\\
& \frac{x-l}{u-l} \text{ if } l\le x\le u\\
& 1, \text{ if } x>u 
\end{align*}\right.$$
The mean is simply the midpoint
### The Exponential Distribution

## Discrete Probability Distributions
