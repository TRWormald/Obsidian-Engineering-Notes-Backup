>Suppose that a haulier is contracted to remove 7 tonne average loads of earth from a building site but an unscrupulous site manager is actually aiming for an 8 tonne average. 
>• If you incorrectly accuse the site manager of fraud, you risk the contract 
>• If you incorrectly believe the loads to be the right weight, you lose money on costs 
>How do you investigate using hypothesis testing?

![[Pasted image 20250410152925.png]]
**What can we change to improve matters?**
- **Effect Size** - how big an effect do we care about
	- Probably don't care about being 1kg over the limit.
- **Sample Size** - how many observations can we make?
	- Usually keep this small to reduce costs, but how small?
- **Significance** - how many false positives do we case about?
	- It depends on what's at stake
- **Statistical Power** - how many false negatives do we care about?
	- $\text{Statistical Power}=1-P(\text{Type-2 Error})$
Prescribe three of the factors and the fourth is determined.
>We’ve seen that an effect size of one (the true mean is one tonne greater than the null hypothesis mean) gives a statistical power of 1-0.74 = 0.26 How big would the effect size need to be give a statistical power of 80%?
### Improving Discrimination by Changing the Sample Size
![[Pasted image 20250410153810.png|centre]]
![[Pasted image 20250410153821.png|centre]]
![[Pasted image 20250410153835.png|centre]]
![[Pasted image 20250410153850.png|centre]]
So as we increase the sample size the false negative rate decreases, meaning that we aren't falsely accepting the base case as often, however we also aren't increasing our chances of getting a false positive.
**But what have our assumptions been?**
In this example we know the ground truth — in practice you don’t Power analysis relies on knowing the shape distribution of the alternative hypothesis 
-  If you are looking at mean values of a sufficiently large sample you can assume a normal distribution because of the central limit theorem 
- Sometimes you just assume the same distribution as the null hypothesis…
- Sometimes you can’t assume anything…