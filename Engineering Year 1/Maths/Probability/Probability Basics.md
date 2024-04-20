Probability theory measures the chance of a random **event** happening.
\
For each **event** we have to consider the sample space $S$ - this is the set of **all possible outcomes**; ultimately events are a subset of the sample space.
\
Often we can represent sets on a Venn diagram!
#### Common Notation
This is an **or** symbol $\cup$ it is used when you want the areas of two sets combined:
$$P(A\cup B)\text{ is the probability of A or B happening}$$
This is an **and** symbol $\cap$ it is used when you want the intersection of two sets:
$$P(A\cap B)\text{ is the probability of A and B happening}$$
When a set has a bar over the top $\bar{x}$ it means **not**, so in this case $\bar{x}=1-x$.
#### Independence and Mutual Exclusivity
##### Idependance
If two (or more) events are independent then they do not effect each other in any way, an example of this would be tossing a coin - it coming up heads the first time has no impact on what it will come up the next time.
For two events to be independent they must satisfy the following equation:
$$P(A\cap B)=P(A)P(B)$$
#### Mutual Exclusivity
If two (or more) events are mutually exclusive they cannot occur at the same time - for example a coin cannot be both heads and tails in a single toss.
Mutually exclusive events abide by the following:
$$P(A\cap B)=0$$
### Conditional Probability
Conditional probability is where you are finding the probability of an event occurring given the fact that another event has occurred. The following notation is used:
$$P(A|B)\text{ this is the probability of A given B}$$
For conditional events the following formula is used:
$$P(A|B)= \frac{P(A\cap B)}{P(B)}$$
It is important to note that $P(A|B)\neq P(B|A)$.    
#### Bayes' Theorem
This leverages the equation for conditional probability in the following way:
$$P(A|B)=\frac{P(A\cap B)}{P(B)}~~~\text{and}~~~P(B|A)=\frac{P(B\cap A)}{P(A)}$$
$$\text{And since } P(A\cap B)=P(B\cap A)$$
$$P(A|B)~P(B)=P(B|A)~P(A)$$
$$\boxed{P(B|A)=P(A|B)\frac{P(B)}{P(A)}}$$
