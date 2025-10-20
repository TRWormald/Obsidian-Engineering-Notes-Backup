## Covariance
### Bivariate Normal Distribution
For a bivariate normal distribution all you need to specify the mean $\mu$ of each random variable and the *covariance matrix $\Sigma$*:
$$(X,Y)\sim N(\mu,\Sigma)=N\left(\begin{bmatrix}\mu_{X}\\\mu_{Y}\end{bmatrix},\begin{bmatrix}\sigma_{X}^{2}&\sigma_{X,Y}\\\sigma_{X,Y}&\sigma^{2}_{Y}\end{bmatrix}\right)$$
The variances are defined as normal (using expected values):
$$\sigma_{X}^{2}=E[(X-\mu_{X})^2]$$$$\sigma_{Y}^{2}=E[(Y-\mu_{Y})^2]$$
and the covariance $\sigma_{X,Y}$ is given by:
$$\sigma_{X,Y}=E[(X-\mu_{x})(Y-\mu_{Y})]$$
*Note that you need to increase the dimensions of $\mu$ and $\Sigma$ for multi-variate normal distributions.*

The covariance matrix tells us about the links (at a linear level) between two (or more) random variables.
![[Pasted image 20250412123000.png|centre]]
### Sampling - Covariance
![[Pasted image 20250412123058.png|centre]]
![[Pasted image 20250412123110.png|centre]]
![[Pasted image 20250412123240.png|centre]]
![[Pasted image 20250412123254.png|centre]]
## Correlation
A normalisation of the covariance gives us the correlation:
$$\rho:=\frac{\sigma_{X,Y}}{\sigma_{X}\sigma_{Y}}~~~\text{such that}~~~-1\le\rho\le 1$$
This is called Pearson's Correlation Coefficient. It tells us the linear correlation between two random variables.
This is defined at the level of the population, not individual samples, and so it is a deterministic quantity.
![[Pasted image 20250412125412.png|centre]]
### Sampling - Correlation
A sample estimate for the correlation coefficient can also be determined. The sample correlation coefficient is:
$$r=\frac{q_{X,Y}}{s_{X}s_{Y}}$$
Expanding this out gives:
![[Pasted image 20250412133326.png|centre]]
The sample correlation coefficient is a random variable whose distribution is known when the input data is bivariate normal.
### Hypothesis Testing With Correlation
Sometimes it is useful to be able to test the hypothesis that data is not correlated - is there correlation in the data below?
![[Pasted image 20250412152046.png|centre]]
#### Sample Correlation Test Statistic
We could use the value of $r$ directly as our test statistic, and do a two-tailed test on whether $r$ is non-zero. The exact distribution of $r$ is horrible, and so we use a transformation instead.

**The Fisher Transformation** turns the sample correlation coefficeint $r$ into an approximately normally distributed random variable:
$$\frac{1}{2}\ln\left(\frac{1+r}{1-r}\right)\sim N\left(\frac{1}{2}\ln\left(\frac{1+\rho }{1-\rho }\right),\frac{1}{n-3}\right)$$
Where $\rho$ is the true or population correlation coefficient and $n$ is the number of samples.
Transforming this into a standard normal gives:
![[Pasted image 20250412152354.png|centre]]
#### Example
![[Pasted image 20250412152423.png|centre]]
#### Exercise
![[Pasted image 20250412152438.png|centre]]
## Linear Regression
**What can we use regression for?**
Finite element simulations are slow, and therefore we can use a *surrogate model* for quick computation, and the full model for final testing (Also known as a metamodel, reduced order model or emulator).
![[Pasted image 20250412152636.png|centre]]
Linear regression is a means for estimating the parameters of a model of the form:
$$y=\beta_{1}u_{1}+\beta_{2}u_{2}+...+\beta_{p}u_{p}$$
Where $y$ is the dependent (output) variable, $u_{i}$ are the independent input variables, and $\beta_{i}$ are the parameters to be estimated.
This model is linear in the parameters; it can be that the model is nonlinear in terms of the independent variables! For example:
$$y=\beta_{1}x+\beta_{2}x^{2}+\beta_{3}x^{3}$$
Hence with linear regressions, $y$, and $x_{i}$ are known from $n$ different samples. Hence we have:
![[Pasted image 20250412153158.png|centre]]
Which is:
![[Pasted image 20250412153236.png|centre]]
In matrix form.
#### Minimising Error
For a particular choice of $\beta$ construct the residual or error vector:
![[Pasted image 20250412153310.png|centre]]
What choice of $\beta$ minimises the error.
First, what is meant by small since the error is a vector? The obvious answer is the Euclidian norm:
$$||e||=\left(\sum\limits_{i}e_{i}^{2}\right)^{\frac{1}{2}}$$
Which gives us least-squares.
#### Ordinary Least Squares
Ordinary least squares corresponds to minimising the error in the $y$ direction - errors in the $x$ direction are ignored.
![[Pasted image 20250412153511.png|centre]]
Minimising the error term corresponds to finding $\beta$ such that:
$$\frac{d||e||}{d\beta_{i}}=0,~~\text{for }i=1,...,p$$
Take the simple example of fitting a straight line:
$$y=\beta_{1}+\beta_{2}x$$
Here we have:
$$||e||^{2}=\sum\limits_{i=1}^{n}(y_{i}-\beta_{1}-\beta_{2}x_{i})^{2}$$
Note that minimising $||e||^{2}$ gives the same result as minimising $||e||$ in this context.
![[Pasted image 20250412153719.png|centre]]
#### Errors in the $x$ direction
We've assumed no errors in the $x$ direction - swapping the $x$ and $y$ coordinates gives different answers:
![[Pasted image 20250412153813.png|centre]]
The only time what we get the same results when we swap $x$ and $y$ is when there is perfect correlation between $x$ and $y$, i.e. $r=\pm 1$.
If we have two least square fits:
$$y=\beta_{1}+\beta_{2}x$$
$$x=\hat{\beta}_{1}+\hat\beta_{2}y$$
Then its possible to show that:
$$\beta_{2}\cdot \hat\beta_{2}=r^{2}$$
Hence:
$$\beta_{2}=1/\hat\beta_{2}$$
Only when $r=\pm 1$.
#### Exercise
![[Pasted image 20250412154047.png|centre]]

#### Under What Conditions Can We Use Linear Regression
1) Normal residuals
2) Constant variability (homoscedasticity)
3) Independence of observations
##### Normal Residuals
The residuals are:
$$e_{i}=y_{i}-\sum\limits_{j}\beta_{j}x_{i,j}$$
i.e. the difference between the line of best fit and the actual observation.
Plot a histogram of residuals:
![[Pasted image 20250412154440.png|centre]]
##### Constant Variability
There should not be any obvious trends in the residuals (should be normal random variables) and variability (e.g. standard deviation) should not change as the independent variables does.
Plot the residuals against the independent variable:
![[Pasted image 20250412154508.png|centre]]
##### Independence of Observations
There should not be any obvious trends in the residuals (should be normal random variables) and the value of each residual should not depend on another.
Plot the $i$-th residual against the $i+1$-th residual.
![[Pasted image 20250412154632.png|centre]]
#### Least Squares with Arbitrary Functions
Often data contains non-polynomial trends that we want to investigate:
![[Pasted image 20250412154723.png|centre]]
![[Pasted image 20250412154742.png|centre]]
![[Pasted image 20250412154753.png|centre]]

#### The General Approach
![[Pasted image 20250412154809.png|centre]]
![[Pasted image 20250412154836.png|centre]]
![[Pasted image 20250412154847.png|centre]]
#### Exercise
![[Pasted image 20250412154905.png|centre]]


