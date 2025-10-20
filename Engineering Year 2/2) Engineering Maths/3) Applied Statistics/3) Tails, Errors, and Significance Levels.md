In an ideal world we'd be able to calculate the probability of the model occurring given the outcome that we have (i.e. $P(\text{model}|\text{outcome})$)
However we can only calculate the probability of the outcome occurring given the model (i.e. $P(\text{outcome}|\text{model})$).
If the probability is small, the implication is that the model is not true since the outcome did occur (However the converse to that doesn't work.)
### One vs Two Tailed Tests
When hypothesis testing we can use one or two tailed tests.
One tailed tests allow us to determine whether the values are higher or lower than expected.
Two tailed tests allow us to determine whether there is any deviation from the normal
![[Pasted image 20250410143739.png|centre]]
### Significance
The question is where do we draw the line?
At what p-value do we reject the null hypothesis $H_0$?
This in fact depends on the distribution of the alternate hypothesis $H_{A}$.
![[Pasted image 20250410143900.png|centre]]
Because having the incorrectly selected level of significance can result in errors, namely:
1) Type 1 (false positive) - incorrectly reject $H_{0}$
2) Type 2 (false negative) - incorrectly accept $H_{0}$
**Errors are always possible!**
Type 1 errors occur at the same rate of significance level.
	This error only occurs when the null hypothesis is true — we know the distribution better than 50% chance of error occurring within 14 experiments if 5% significance used
Type 2 errors occur at unknown rates.
>Most of the time we use 5% as the level of significance, **however it is not necessarily always the answer, we instead have to balance the Type 1 and Type 2 errors to select the correct significance level.**