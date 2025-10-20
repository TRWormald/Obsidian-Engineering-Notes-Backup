Hypothesis testing is a method of testing a "belief" (or base case) about the world.
Effectively we have:
1) A model of the world
2) Observations of the world
And we want to know how well the observations fit the model.
#### Example
Say we are calculating the probability that there are no black jurors on a jury in the 1900s. (See lecture slides for more info).
Our given distribution is:
$$X\sim B(12,0.25)$$
Hence we get:
![[Pasted image 20250410143117.png|centre]]
Getting:
$$P(X=0)=0.75^{12}=0.031676$$
So 3.2% of the time we would expect to see 12 white jurors.
**However how do we know whether the model is wrong (i.e. how do we know the result is statistically *significant***.