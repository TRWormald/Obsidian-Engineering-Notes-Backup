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
The mean is simply the midpoint:
$$\mu =\frac{u+l}{2}$$
And the variance is calculated as follows:
$$\sigma^{2}=\frac{(u-l)^{2}}{12}$$
### The Exponential Distribution
The exponential distribution $e^\lambda$ is a continuous distribution with mean $\mu=1/\lambda$ and variance $\sigma^{2}=1/\lambda^{2}$, below is a graph of its PDF:
![[Pasted image 20240420165042.png|center|400]]
Which is represented by the equation:
$$f_{X}(x)=\left\{\begin{align*}
& \lambda e^{-\lambda x }\text{ if } x\ge0\\
& 0 \text{ otherwise}
\end{align*}\right.$$
And the CDF is as follows:
$$F(x)=\left\{\begin{align*}
& 0,\text{ if } x<0\\
& 1-e^{-\lambda x} \text{, if } x\le0
\end{align*}\right.$$
## Discrete Probability Distributions
We can also have random variables $X$ that take on discrete values, like with a coin toss (binary) or a dice roll (1,2,3,4,5,6)
The set $S$ must be countable - i.e. it must be able to be labelled by a subset of the natural numbers.
Each outcome must have a finite probability $P(X=x)$
##### Fair Dice Example
Consider a fair six sided dice, we will define a probability mass function (PMF - as opposed to the PDF of a continuous distribution)
For it to be valid:
$$\sum\limits_{x\in S}P_{X}(x)=1$$
So for our die:
$$P_{X}(x)=\left\{\begin{align*}
& \frac{1}{6},\text{ if } x\in S=[1,2,3,4,5,6]\\
& 0 \text{, otherwise }
\end{align*}\right.$$
### CDF, Mean (Expectation) and Variance
The CDF, Mean, and Variance of discrete distributions are very similar to their continuous counterparts.
The CDF is the same as the continuous case but replaces the $\int$ with a $\sum$:
$$F_{X}(x)=P(X\le x)=\sum\limits_{k=1}^{x}P(X=k)$$
The mean (expectation) is the same:
$$\mu=E(X)=\sum\limits_{x\in S}xP_{X}(x)$$
And the same is again true of the variance:
$$\begin{align*}
\sigma^{2}=E[(X-\mu)^{2}]&= \sum\limits_{x\in S}(x^{2}-2\mu x+\mu^{2})P_{X}(x)\\
&= \sum\limits_{x\in S}x^{2}P_X(x)-2\mu\sum\limits_{x\in S}xP_X(x)+\mu^{2}\sum\limits_{x\in S}P_X(x)\\
&= E(X^{2})-2\mu^{2}+\mu^{2}\\
&\boxed{= E(X^{2})-\mu^{2}}
\end{align*}$$
### The Bernoulli Distribution
In the Bernoulli Distribution we denote the success probability as $p$ and therefore the failure probability must be $1-p$.
Let $X$ be the random variable that equals one if the outcome is a success, and 0 if it is a failure.
Therefore the probability function is:
$$P_{X}(1)=P(X=1)=p$$
$$P_{X}(0)=P(X=0)=1-p$$
This is the simplest possible probability distribution to a truly random experiment.
### The Geometric Distribution
Let the random variable $X$ be the number of trials until (and including) the first success.
If $X=n$, then we must have $(n-1)$ failures followed by 1 success.
All trails are independent so we can multiply probabilities:
$$\begin{align*}
P(X=n)&= \underbrace{(1-p)\times(1-p)\times...\times(1-p)}_{n-1\text{ times}}\times p\\
&= (1-p)^{n-1}p
\end{align*}$$
We can show that the mean is given by $\frac{1}{p}$:
$$\begin{align*}
\mu=E(X)&= \sum\limits_{n=1}^{\infty}[nP_{X}(n)]=\sum\limits_{n=1}^{\infty}np(1-p)^{n-1}\\
&= p\sum\limits_{n=1}^{\infty}n(1-p)^{n-1}\\
&= p\left(\sum\limits_{n=1}^{\infty}n(1-p)^{n-1}+\sum\limits_{n=2}^{\infty}n(1-p)^{n-1}+...\right) \\
&= p\left(\frac{1}{p}+\frac{1-p}{p} + \frac{(1-p)^{2}}{p}+...\right)\\
&= p(1+(1-p)+(1-p)^{2}+...)\\
&= \frac{1}{1-(1-p)}=\frac{1}{p}
\end{align*}$$
A similar method gets us the CDF:
$$F_{X}(n)=P(X\le n)=1-(1-p)^{n}$$

