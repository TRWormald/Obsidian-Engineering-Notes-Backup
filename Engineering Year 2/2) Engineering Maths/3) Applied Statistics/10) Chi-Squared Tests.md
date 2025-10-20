
>**Categorical Data**
>Categorical Data is Data that has been broken into categories of some description.

**Injuries to a typical toddler:**
![[Pasted image 20250412111706.png|centre]]
This is *categorical data*.
If there were two categories then we could use a Binomial distribution with a given number of events (say 40) to determine whether a particular toddler is "normal":
![[Pasted image 20250412111814.png|centre]]
**But how can we generalise this to multiple categories?** We have to use a "multinomial" (or categorical distribution).
An example of this is Pearson's Chi-Squared ($\chi^{2}$) test. It is an approximate test that works well for large (and not so large) numbers of measurements. In the limit as $n\rightarrow \infty$ it gives the exact answer.
### Chi-Squared
To set up a $\chi^{2}$ test we:
1) Label observed outcomes as $O_{i}$ where $n=\sum_{i}O_{i}$
2) Label expected outcomes as $E_{i}=n\cdot P_{i}$ where $P_{i}$ are the probabilities of each outcome
![[Pasted image 20250412112318.png|centre]]
The Chi-Squared test states that:
$$\sum\limits_{i=1}^{m}\frac{(O_{i}-E_{i})^{2}}{E_{i}}\sim \chi_{m-1}^{2}$$
Where $m$ is the number of categories.
Our base case ($H_{0}$) is that the toddler is "typical" (i.e. their distribution of accidents follows the nationwide statistics).
$$\chi^{2}=\frac{(140-127)^{2}}{127}+\frac{(20-25.2)^{2}}{25.2}+\frac{(20-11.8)^{2}}{11.8}+\frac{(4-6.4)^{2}}{6.4}+\frac{(16-16.4)^{2}}{16.4}+\frac{(0-13.2)^{2}}{13.2}=22.21$$
There are 6 categories and so there are $6-1=5$ degrees of freedom. The tables give us a critical value of $\chi_{5}^{2}(0.05)=11.070$ and so we reject the null hypothesis. (So our toddler is "a-typical")
![[Pasted image 20250412113047.png|centre]]
### Exercise 1
![[Pasted image 20250412113116.png|centre]]
### Independence Testing
We can also use Pearson's $\chi^{2}$ test for testing independence.
e.g. "Are men and women aged 15-65 equally accident prone?":
![[Pasted image 20250412113214.png|centre]]
We assume that males/females have the same probabilities for an injury (our base case) to calculate the expected values:
![[Pasted image 20250412113347.png|centre]]
So we have totalled the number of injuries for each mechanism and taken the probability as a fraction of total injuries.
**The degrees-of-freedom** is given by $(\text{rows}-1)\times(\text{columns}-1)=(5-1)(2-1)=4$
Calculating things from the data (the probabilities) adds constraints, which reduce the number of degrees of freedom.

Our test statistic is the same as before, leading to:
![[Pasted image 20250412113637.png|centre]]
The critical value for $\chi^{2}_{4}(0.05)=9.488<52.05$ hence we reject $H_{0}$.
Which means that there is a statistically significant difference between men and women with regards to the accidents they have.
### Exercise 2
![[Pasted image 20250412113746.png|centre]]
### Goodness-of-Fit Testing
Finally, we can also use Pearson's $\chi^{2}$ test to determine if data is taken from a particular distribution (e.g. normal or Poisson).
For example using the following data on "Days spent in hospital following an accident for children aged 5-14 years":
![[Pasted image 20250412113919.png|centre]]
Does the data follow a Poisson distribution?

First we need to calculate the mean from the data (this is all that is needed for a Poisson - using a Normal distribution we would need to calculate the standard deviation as well)

Use the midpoints of the intervals for the calculations:
![[Pasted image 20250412114049.png|centre]]
and the mean can then be used to generate expected values from the Poisson distribution:
![[Pasted image 20250412114140.png|centre]]

Pearson's $\chi^{2}$ test is only an approximate test, to work as expected each of the expected values should be greater than 5. Any categories with smaller numbers should be merged together.
The final table is thus:
![[Pasted image 20250412114240.png|centre]]
With the final calculation being:
![[Pasted image 20250412114413.png|centre]]
The number of degrees of freedom can be calculated to be:
$$\text{DOF}=\text{No. of Categories }-\text{No. of Calculated Quantities }-1$$
So in this case that's 3-1-1=1. Hence:
$$\chi^{2}(0.05)=3.841$$
Which is less than our calculated value of 65.5 and therefore we need to reject $H_{0}$. (Meaning that the data doesn't follow the Poisson distribution)
### Exercise 3
![[Pasted image 20250412115437.png|centre]]

