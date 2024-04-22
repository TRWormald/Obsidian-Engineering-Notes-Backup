### Mean
The mean is the average value of the data, it is calculated in the following way:
$$\text{Mean}=\mu=\frac{1}{N}\sum\limits_{i=1}^{N}x_i$$
Where $N$ is the number of data points.
#### Finding the mean of a Continuous Distribution
Under the "law of averages" we expect a random process to settle as we take lots of observations.
The mean of a probability distribution $X$ is written $\mu=E(X)$ - where $E(X)$ is the **expected value of X**.
This can be calculated as:
$$\mu=E(X):=\int_{-\infty}^{\infty}\tilde{x}\cdot f_{X}(\tilde{x})\cdot d\tilde{x}$$
So we are integrating over all possible values that $X$ can take and multiplying each of those values by the probability of that event.
### Standard Deviation
Standard deviation is a measure of how the data varies around the mean, with a larger standard deviation representing a greater spread of values.
It is calculated in the following way:
$$\text{Standard Deviation}=\sigma=\sqrt{\dfrac{\sum\limits_{i=1}^{N}x^{2}_{i}}{N}-\left(\dfrac{\sum\limits_{i=1}^{N}x_{i}}{N}\right)^{2}}$$
One way to remember the equation is that it is the *"Square root of the mean of the squares minus the square of the mean"*.
\
The standard deviation is also the square root of the variance $\sigma^{2}$ - sometimes called $\text{Var(X)}$ which is a measure of how a distribution deviates from its mean. It is equal to:
$$\sigma^{2}=E[(X-\mu)^{2}]$$
So for continuous distributions:
$$\begin{align*}
E[(X-\mu^{2})]:&= \int_{-\infty}^{\infty}(\tilde{x}-\mu)^{2}f_{X}(\tilde{x})\cdot d\tilde{x}\\
&= \int_{-\infty}^{\infty} \tilde{x}^{2}f_{X}(\tilde{x})\cdot d\tilde{x}-2\mu\underbracket{\int_{-\infty}^{\infty}\tilde{x}f_{X}(\tilde{x})\cdot d\tilde{x}}_{=\mu}+\mu^{2}\underbracket{\int_{-\infty}^{\infty}f_{X}(\tilde{x})\cdot d\tilde{x}}_{=1}\\
&= \int_{-\infty}^{\infty} \tilde{x}^{2}f_{X}(\tilde{x})\cdot d\tilde{x} -2\mu^{2}+\mu^{2}\\
&= \int_{-\infty}^{\infty} \tilde{x}^{2}f_{X}(\tilde{x})\cdot d\tilde{x} -\mu^{2}\\
&= E(X^{2})-\mu^{2}
\end{align*}$$
If we think about what's happened here, all we've really done is rewritten the equation for standard deviation in continuous form.
As:
$$\int_{-\infty}^{\infty} \tilde{x}^{2}f_{X}(\tilde{x})\cdot d\tilde{x}$$
Is the mean of the $\tilde{x}$ values, or "the mean of the squares", and then we subtract the "square of the mean".
