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
