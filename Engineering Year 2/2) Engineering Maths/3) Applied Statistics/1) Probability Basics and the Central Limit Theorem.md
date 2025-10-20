**The Normal Distribution is the Bedrock of Probability**
Below is a normal distribution:
![[Pasted image 20250205170435.png|centre|350]]
The distribution function is:
$$X\sim N(\mu,\sigma ^{2})$$
And the probability density function is:
$$f_{X}(x)=\frac{1}{\sigma \sqrt{2\pi}}e^{-\frac{1}{2}\left(\frac{x-\mu}{\sigma}\right)^{2}}$$
Where the PDF gives the value of $f_{X}$ at a given $x$.
****
The CDF (or cumulative density function) is the probability of $X\le x$ and can be calculated using:
$$\Pr(X\le x)=F_X(x)=\int_{-\infty}^{x}f_{x}~dx$$
![[Pasted image 20250205171148.png|centre|350]]
### The Standard Normal
We can also define the standard normal, which is where we set the standard deviation to one and the median to zero to be able to compare distributions.
This is done by subtracting and dividing.
### The Sum of Two Normal Variables
Given two normally distributed variables:
$$X_{1}\sim N(\mu_{1},\sigma_{1}^{2})~~~\text{and}~~~X_{2}\sim N(\mu_{2},\sigma_{2}^{2})$$
Their sum $X_{1}+X_{2}$ is also normally distributed
$$X_{1}+X_{2}\sim N(\mu_{1}+\mu_{2}, \sigma_{1}^{2}+\sigma_{2}^{2}) $$
As is their difference $X_{1}-X_{2}$
$$X_{1}-X_{2}\sim N(\mu_{1}-\mu_{2}, \sigma_{1}^{2}+\sigma_{2}^{2})$$
### The Central Limit Theorem
Given the previous rules, the mean of $n$ independent identically distributed variables $X_{i}\sim N(\mu,\sigma^{2})$ is:
$$\bar{X}=\frac{1}{n}\sum\limits_{i=1}^{n}X_{i}\sim N\left(\mu,\frac{\sigma^{2}}{n}\right)$$
The mean is a random variable itself with it's own distribution.
Notice how the variance of the mean decreases with the increasing number of observations.
*Note that this does not mean that all means are normally distributed.*
#### The Sample Mean
The sample mean is the mean value of a sample of a population, for example average height:
![[Pasted image 20250410140659.png|centre]]
The Sample Mean of the above is 1.65, but the mean of another sample of the same population might be different:
![[Pasted image 20250410140753.png|centre]]
#### Distribution of the Sample Mean for Non-Normal Random Variables
In general when we have two random variables, e.g. $X_{1}$ with pdf $f(x)$ and $X_{2}$ with pdf $g(x)$
The distribution of their sum is:
$$Y=X_{1}+X_{2}$$
with pdf:
$$(f\cdot g)(x)$$
Where $(f\cdot g)$ is the convolution integral:
$$(f\cdot g)(x)=\int_{-\infty}^{\infty}f(x-t)g(t)\cdot dt$$
(Which we don't have to solve, only approximate numerically)
#### The Central Limit Theorem
There is a very useful theorem that comes to our rescue:
>Given a random sample of $n$ independent and identically distributed random variables ${X_{1},...,X_{n}}$, each with mean $\mu$ and variance $\sigma^{2}$, the sample mean:$$\bar{X}=\frac{1}{n}\sum\limits_{i=0}^{n}X_{i}$$Is normally distributed such that:$$(\bar{X}-\mu)\sqrt{n}\sim N(0,\sigma^2),~~~~n\rightarrow\infty$$Hence for large (but finite) $n$ we have that $\bar{X}$ is approximately distributed as $N(\mu,\sigma^{2}/n)$ **But it says nothing about the individual $X_{i}$ values!**

It is possible to use the central limit theorem if:
1) $n\ge 25$ and the underlying distribution is approximately symmetric
2) $n\ge 100$ and the underlying distribution is strongly skewed
For finite $n$ the central limit theorem gives the approximate distribution - with a higher $n$ giving a better approximation.