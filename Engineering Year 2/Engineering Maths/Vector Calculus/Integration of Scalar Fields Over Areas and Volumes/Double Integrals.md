E.g. calculate the mass of a lamina occupying a region $R$ in the $(x,y)$-plane, whose density variation is $\rho(x,y)$.
$$\text{Area of R}=\int\int_{R}dA=\int\int_R dx~dy$$
Therefore:
$$\text{Total Mass}= \int\int_{R}\rho(x,y)~dx~dy$$
This is an example of a double integral which we interpret as representing the volume under the 'height function' $f(x,y)$ above the region $R$:
![[Pasted image 20241015211934.png|centre]]
Effectively we are multiplying each of thee infinitesimal areas making up $R$ by the height at that specific point, giving us the volume.
\
Such integrals are calculated by first integrating with respect to one variable, then the other. According to notation we do the inner integral first:
$$\int\int f(x,y)~dx~dy=\int\left[\int f(x,y)~dx\right]dy$$
#### Example 5.1
![[Pasted image 20241015212214.png|centre]]
![[WhatsApp Image 2024-10-15 at 21.29.27_14ec6128.jpg|centre]]
### The Area of a General Region
In [[Double Integrals#Example 5.1|5.1]] the area was obviously a rectangle, so the limits on $x$ and $y$ were obvious. But what are the limits on $x$ and $y$ for a general region $R?$
Here it matters in which order we perform the integration.
Suppose we perform the integration with respect to $x$ first, as in 5.1. Then we should express the region $R$ in the form:
$$R: c\le y\le d~~~~~~~p(y)\le x\le q(y)$$
Then:
$$\int\int_{R} f(x,y)~dx~dy=\int_{y=c}^{d}\left[\int_{x=p(y)}^{q(y)} f(x,y)~dx\right]dy$$
And the inner integral is:
$$\int_{x=p(y)}^{q(y)}f(x,y) ~dx:=P(y)$$
Which for $y$ is just a constant, has limits which may be (and in general are) functions of $y$.
Physically we are summing the area under the curve along thin vertical strips of width $dy$, of length $q-p$:
![[Pasted image 20241015214644.png|centre]]
The outer integral is now:
$$\int_{y=c}^{d}P(y)~dy$$
Which is not a function of $x$ or $y$, so its limits are constants. This is the sum of all the horizontal strips between $y=c$ and $y=d$.
\
**More generally what we are doing is generating a function in terms of $y$ for the width of the horizontal strips and then integrating that w.r.t the vertical axis's limits.**
#### Example 5.2
![[Pasted image 20241015213005.png|centre]]![[WhatsApp Image 2024-10-15 at 21.40.37_054acf04.jpg|centre]]
#### Example 5.3
![[Pasted image 20241015215154.png]]
![[WhatsApp Image 2024-10-15 at 22.10.53_de10313b.jpg|centre]]
### Properties of Double Integrals
The following are some obvious relationships for double integrals:
**Linear** - If $\alpha$ and $\beta$ are constant scalars:
$$\int\int_{R}(\alpha f(x,y)+\beta g(x,y))~dx~dy=\alpha\int\int_{R}f(x,y)~dx~dy+\beta\int\int_{R}g(x,y)dx~dy$$