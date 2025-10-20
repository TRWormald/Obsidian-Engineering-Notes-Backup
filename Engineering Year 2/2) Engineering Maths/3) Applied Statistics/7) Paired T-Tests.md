>Is a new fitness regime better than the old one?
>A coach assesses two regimes using a step test and measuring pulse rate:![[Pasted image 20250410173844.png]]

Ideally we'd have more data to show trends over time.
We could average the results to produce an aggregate value for the new regime versus the old regime and use a hypothesis test, but this wouldn't work as intended due to:
- Variability between individuals is potentially larger than the difference caused by the change of regime
- Samples are not independent - underlying physiology of the individuals doesn't change

>Given this particular example of testing fitness regimes, what other confounding factors could be important? Make a list and see how many you can come up with

**This is paired data** which is common in before-and-after statistical trials, e.g. drugs trials.
Summary statistics:
-  Biggest decrease: person E (from 105 to 96 beats per minute) 
-  Biggest increase: person C (from 80 to 86 beats per minute) 
-  Highest heartbeat: person G (110 beats per minute) 
-  Lowest heartbeat: person F (62 beats per minute)

**Now lets calculate the difference in pairs for each individual:**
![[Pasted image 20250410174220.png|centre]]
Now each $X_{\Delta}$ is independent of each other.
The null hypothesis can be stated to be that the new fitness regime is the same as the old one:
$$H_{0}:\bar{X}_\Delta=0$$
Using the standard T-Test statistic:
$$T=\frac{\bar{X}_{\Delta}}{\frac{s_{\Delta}}{\sqrt{n_{\Delta}}}}\sim T_{n_{\Delta}-1}$$
Where:
$$\bar{X}_\Delta=\frac{1}{n_{\Delta}}\sum X_{\Delta},~~s_{\Delta}^{2}=\frac{1}{n_{\Delta}-1}\sum(X_{\Delta}-\bar{X}_{\Delta})^{2}$$
And $n_{\Delta}$ is the number of pairs.
Fitness data gives: $\bar{X}_{\Delta}=-3.1$, $s_{\Delta}=5.1$, and $n_{\Delta}=10$.
Therefore:
$$T=\frac{-3.1}{5.1/\sqrt{10}}=-1.92$$
The critical value is $T_{9}(0.05)=1.833$ (one-tailed) so we can reject $H_0$.
### When is Something Insignificant Significant
Statistical significance tends to occur when either there are:
1) Many observations and a small deviation from the hypothesis
2) A few observations and a large deviation from the hypothesis
**Don't confuse statistical significance (or lack thereof) for practical significance (or lack thereof)**
A moderate deviation may not be detected with only a few deviations. Is a small deviation of practical significance?
### Failing to Reject the Null Hypothesis
The 1973 oil crisis led to traffic agencies considering whether to allow vehicles to turn right at a red light (USA). There were significant safety concerns and a number of studies performed. 
A consultant in Virginia conducted a before-and-after study of 20 intersections. 
**Before** there were 308 accidents and 
**Afterwards** there were 337 accidents in a similar time frame. 

This result was not statistically significant. The final report to the governor stated we can discern no significant hazard to motorists or pedestrians from the implementation Practical significant = statistical significance?!

These studies were **underpowered** - they were not sufficiently sensitive to the phenomenon they were trying to measure! Subsequent studies have found:
- 20% increase in collisions, 
- 60% more pedestrians being run over, and 
- Twice as many bicyclists being struck!

Just because you can’t reject your hypothesis doesn’t mean it’s right!
