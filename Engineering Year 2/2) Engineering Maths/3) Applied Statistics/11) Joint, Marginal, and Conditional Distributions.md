So far we've considered a single random variable:
- Either a continuous random variable, or
- A discrete random variable (categories)

What happens when we have more than one random variable?

The simplest case is one where we have independent random variables:
$$P(A \text{ and } B)=P(A)P(B)$$
A more difficult case is then the random variables are dependent:
$$P(A \text{ and } B)=P(A)P(B|A)=P(A|B)P(B)$$
### Exam Results Example:
![[Pasted image 20250412120233.png|centre]]
### Independent Normal - Joint Distribution
![[Pasted image 20250412120514.png|centre]]
![[Pasted image 20250412120651.png|centre]]
### Covariant Normal - Joint Distribution
![[Pasted image 20250412120707.png|centre]]
![[Pasted image 20250412120725.png|centre]]
### The Joint Distribution
The joint distribution $p_{X,Y}(x,y)$ is the key distribution from which all others can be derived:
$$P((a_{X}\le X\le b_{X})~~\text{and}~~(a_{Y}\le Y\le b_{Y}))=\int_{a_{X}}^{b_{X}}\int_{a_{Y}} ^{b_{Y}}p_{X,Y}(x,y)~dy~dx$$
If the random variables $X$ and $Y$ are independent, then we have that:
$$P((a_{X}\le X\le b_{X})~~\text{and}~~(a_{Y}\le Y\le b_{Y}))=P(a_{X}\le X\le b_{X})P(a_{Y}\le Y\le b_{Y})$$
Which implies that:
$$p_{X,Y}(x,y)=p_{X}(x)p_{Y}(y)$$
**But this is only for independent random variables**.
### The Marginal Distribution
The marginal distribution is the distribution of one of the variables, ignoring what the other variable is doing. To find it, integrate over all values of the other variable.
$$p_{X}(x)=\int_{y}p_{X,Y}(x,y)~dy$$
This is called marginalisation.
This name comes from having two discrete random variables and writing out the probabilities of all possibilities in a table. The sums of the rows/columns (which give the marginal distribution) end up being written in the margins.
#### Example
![[Pasted image 20250412121527.png|centre]]
### The Conditional Distribution
The conditional distribution is the distribution for one variable when the other variable takes a specific value. That is:
$$p_{X}(x|Y=y)=\frac{p_{X,Y}(x,y)}{p_Y(y)}$$
Where $p_{Y}(y)$ is the marginal distribution.
At one level this concept is relatively easy, but it's not as straightforward as it seems (see the Borel's paradox) - we'll stick with the intuitive definition.
#### Example
![[Pasted image 20250412122245.png|centre]]
