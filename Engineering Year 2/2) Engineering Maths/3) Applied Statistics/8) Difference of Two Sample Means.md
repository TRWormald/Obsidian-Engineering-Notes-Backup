>**Does life experience affect investor decisions?**
>In an attempt to determine whether life experience affects the quality of investment decisions, a research gives £100 to 20 people; 9 are 18–23 years old and 11 are 60–65 years old and asks them to invest the money in shares.
>None of the people involved have any investment experience.
>After 12 months, the returns on their investments are compared.
>![[Pasted image 20250411190536.png|centre]]
>**Summary Statistics:**
>**Extremes** 
>• Person F (18–23 years): £168 
>• Persons R & S (60–65 years): £53 
>**Means** 
>• 9 people 18–23 years, mean of 106.4, s.d. of 37.3 
>• 11 people 60–65 years, mean of 95.7, s.d. of 39.4

First we need to take the sample mean distributions for both groups:
$$\bar{X}_{y}\sim N(\mu_{y},\sigma^{2}_{y}/n_{y})~~\text{Sample Mean for the Young}$$
$$\bar{X}_{o}\sim N(\mu_{o},\sigma^{2}_{o}/n_{o})~~\text{Sample Mean for the Old}$$
We can then calculate the difference (properties of normal distributions):
$$\bar{X}_{\Delta}=\bar{X}_{y}-\bar{X}_{o}\sim N\left(\mu_{y}-\mu_{0},\frac{\sigma_{y}^{2}}{n_{y}}+\frac{\sigma_{o}^{2}}{n_{o}}\right)$$
If we test the hypothesis that $H_{0}:~\bar{X}_{\Delta}=0$ we get:
$$\frac{\bar{X}_{y}-\bar{X}_{o}}{\sqrt{\frac{\sigma_{y}^{2}}{n_{y}}+\frac{\sigma_{o}^{2}}{n_{o}}}}\sim N(0,1)$$
However this assumes that we know the population variances!
As with the T-Test we can substitute in the estimates for the population variances:
$$\frac{\bar{X}_{y}-\bar{X}_{o}}{\sqrt{\frac{s_{y}^{2}}{n_{y}}+\frac{s_{o}^{2}}{n_{o}}}}\sim T_{n-1}$$
But what is the number of degrees-of-freedom $n$? For an accurate answer, use statistical software (it depends slightly on the data). For a simple (conservative) answer, use:
$$n=min(n_{y},n_{o})$$
Answering the question (does life experience affect investing ability) we have:
$$\frac{105.4-97.5}{\sqrt{\frac{37.3^{2}}{9}+\frac{39.4^{2}}{11}}}=0.56$$
Which should be compared against $T_{8}(0.05)=2.306$ (two-tailed). Hence we cannot reject the null hypothesis that both age groups have the same skill at investing...

**NOTE that this shows correlation but not causation.**
When trying to combine features (age and investing ability) be careful of the conclusions you draw If we had rejected the null hypothesis then we could say that the 18–23 year olds higher return on investments was statistically significantly 
- This does not mean being younger makes you a good investor 
- Nor does it mean that being a bad investor indicates you are older
- Lots of different ways this link could materialise