A Semi-Infinite body is formed of a [[Uniform Horizontal Flow]] and a Point Source (See: [[Point Source & Sink]]):
\
![[Pasted image 20240220161147.png]]
\
We know the steps required to solve this kind of problem (See: [[How to solve Potential Flows]]), so the first step should be obtaining the velocity field via [[Laplace's Equation]].
However, before that we should draw a diagram of the problem:
\
![[Pasted image 20240220162106.png]]
\
#### Step 1 - Obtain the Velocity Field
From the potential functions for [[Uniform Horizontal Flow]] and [[Point Source & Sink]] we can calculate that:
\
$$ u=U_\infty + \frac{\Lambda}{2\pi}\frac{x}{x^2+y^2}~,~v=\frac{\Lambda}{2\pi}\frac{y}{x^2+y^2}$$
Where:
$U_\infty$ is the freestream velocity
$\Lambda$ is the source strength
\
However it is important to note that this equation is only true for the source at the origin, therefore limiting us to a single source.

#### Step 2 - Find the Stagnation Points
The stagnation points are points where the velocity of the flow is zero.
So $u=0$ and $v=0$, therefore substituting that into our equations gives:
\
$$v=\frac{\Lambda}{2\pi}\frac{y_{stag}}{x_{stag}^2+y_{stag}^2}=0 ~~~~~~~\Rightarrow ~~~~~~~ y_{stag}=0$$
\
$$u=U_\infty + \frac{\Lambda}{2\pi}\frac{x}{x^2+y^2}=0~~\Rightarrow~~ U_\infty+\frac{\Lambda}{2\pi}\frac{1}{x_{stag}}=0~~\Rightarrow~~x_{stag}=-\frac{\Lambda}{2\pi U_{\infty}}$$
#### Step 3 - Link Source Strength to the Ultimate Height of the Body
This can be done easiest by considering the dividing streamline far downstream:
1) All flow must have returned to freestream conditions
2) All mass (or volume as incompressible) from the source must remain within the dividing streamline
3) So inside the dividing streamline flow speed is $U_\infty$ and volume flow rate is $\Lambda$ (the source strength)
Hence:
\
$$Ultimate~Width = \frac{\Lambda}{U_\infty}$$
\
The velocity at any point is therefore:
\
$$V=\sqrt{u^2+v^2}$$
With $u$ and $v$ being functions of $x$ and $y$
 \
 With the speed we can plug it into [[Bernoulli's Equation]] to calculate the pressure at any point within the flow field.
 