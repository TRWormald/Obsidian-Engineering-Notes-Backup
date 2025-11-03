### Lax-Wendroff
The upwind scheme is only first order accurate in space, and is too diffusive. A higher-order scheme is required. A classic scheme in numerical analysis is that due to P.D. Lax and B. Wendroff, published in 1960. This is second order in space and time. Let us again consider the wave equation:
$$\frac{\partial u}{\partial t}+c\frac{\partial u}{\partial x}=0$$
We know:
$$u_{i}^{n+1}=u_{i}^{n}+\Delta t \left.\frac{\partial u}{\partial t}\right|_{i}^{n} +\frac{1}{2}(\Delta t)^{2}\left.\frac{\partial^{2}u}{\partial t^{2}}\right|_{i}^{n}+O(\Delta t^3)$$
Previously the second difference was included in the truncation error; in the Lax-Wendroff method we use it, but second temporal difference is awkward. So the first step is to formulate an expression for:
$$\left.\frac{\partial^{2}u}{\partial t^{2}}\right|_{i}^{n}$$
#### Step 1 - Find an Expression for the Second Temporal Derivative
For the first temporal derivative, we rearrange our PDE:
$$\frac{\partial u}{\partial t}=-c\frac{\partial u}{\partial x}$$
So:
$$\frac{\partial^{2}u}{\partial t^{2}}=\frac{\partial}{\partial t}\left(-c\frac{\partial u}{\partial x}\right)$$
$c$ is constant so:
$$\frac{\partial^{2}u}{\partial t^{2}}=-c\frac{\partial}{\partial t}\left(\frac{\partial u}{\partial x}\right)=-c\frac{\partial}{\partial x}\left(\frac{\partial u}{\partial t}\right)$$
Then substitute for the first temporal derivative:
$$\frac{\partial^{2}u}{\partial t^{2}}=-c\frac{\partial}{\partial x}\left(-c\frac{\partial u}{\partial x}\right)$$
So we can say that:
$$\frac{\partial^{2}u}{\partial t^{2}}=c^{2}\frac{\partial ^{2}u}{\partial x^{2}}$$
#### Step 2 - Taylor Expansion in Time: Including the Second Derivative Term
Taylor expansion in time:
$$u_{i}^{n+1}=u_{i}^{n}+\Delta t \left.\frac{\partial u}{\partial t}\right|_{i}^{n}+ \frac{1}{2}(\Delta t)^{2}\left.\frac{\partial^{2} u}{\partial t^{2}}\right|_{i}^{n}+O(\Delta t^{3})$$
Then substituting expressions for the first and second derivatives:
$$u_{i}^{n+1}=u_{i}^{n}+\Delta t \left.\left(-c\frac{\partial u}{\partial c}\right)\right|_{i}^{n}+ \frac{1}{2}(\Delta t)^{2}\left.\left(c^{2}\frac{\partial ^{2}u}{\partial x^{2}}\right)\right|_{i}^{n}+O(\Delta t^{3})$$
Or
$$u_{i}^{n+1}=u_{i}^{n}-c\Delta t \left.\frac{\partial u}{\partial c}\right|_{i}^{n}+ \frac{1}{2}c^{2}(\Delta t)^{2}\left.\frac{\partial ^{2}u}{\partial x^{2}}\right|_{i}^{n}+O(\Delta t^{3})$$
We have now developed an expression for the future solution in terms of the first and second spatial derivative. So the next step is to use finite difference formulae for the spatial terms.
#### Step 3 - Finite Differences for First and Second Spatial Derivatives
The forward and backward Taylor expansions in space are:
![[Pasted image 20251031183114.png|centre|400]]
The difference between the two expansions gives us the central difference approximation to this derivative:
$$\left.\frac{\partial u}{\partial x}\right|_{i}^{n}=\frac{u_{i+1}^{n}-u_{i-1}^{n}}{2\Delta x}+O(\Delta x^{2})$$
The sum of the two expansions gives a three-point second order difference approximation to the second derivative, which can be rearranged to obtain:
$$\left.\frac{\partial^{2} u}{\partial x^{2}}\right|_{i}^{n}\simeq\frac{u_{i+1}^{n}-2u_{i}^{n}+u_{i-1}^{n}}{(\Delta x)^{2}}+O(\Delta x^{2})$$
Lastly, substituting our spatial finite differences into our temporal expansion gives the Lax-Wendroff method:
$$u_{i}^{n+1}=u_{i}^{n}-c\frac{\Delta t}{2\Delta x}(u_{i+1}^{n}-u_{i-1}^{n})+ \frac{1}{2}\left(\frac{c\Delta t}{\Delta x}\right)^{2}(u_{i+1}^{n}-2u_{i}^{n}+u_{i-1}^{n})+O(\Delta x^{2}, \Delta t^{2})$$
Hence, the Lax-Wendroff method is second order accurate in both time and space $\rightarrow$ better than simple upwind scheme.

### Stability Analysis of the Lax-Wendroff Method
To tidy the algebra we can start from a point where the exponential in time has been divided through to gain the amplification factor. Increments of $i+1$ or $i-1$ are then just swapped for exponentials in $\Delta x$ of appropriate sign.
$$\lambda=1-\nu\frac{e^{jk\Delta x}-e^{-jk\Delta x}}{2}+\nu^2\frac{e^{jk\Delta x}+e^{-jk\Delta x}-2}{2}$$
Which can be simplified to:
$$\lambda=1-\nu j\sin(k\Delta x)+\nu^{2}(\cos(k\Delta x)-1)$$
$$\lambda ^{2}=(1+\nu^{2}(\cos(k\Delta x)-1))^{2}+\nu^{2}(\sin^{2}(k\Delta x))$$
Which simplifies to:
$$\lambda^{2}=1-2\nu^{2}(1-\cos(k\Delta x))+\nu^{2}(1-\cos^{2}(k\Delta x))+\nu^{4}(1-\cos(k\Delta x))^{2}$$
For the full derivation see [[7) Numerical Methods Lecture 7.pdf#page=11|Numerical Methods Lecture 7, p.11]]. But we eventually obtain:
$$\lambda^{2}=1-4\nu^{2}(1-\nu^{2})\sin^{4}\left(\frac{k\Delta x}{2}\right)$$
### Numerical Example
![[Pasted image 20251031185751.png|centre]]
Lax-Wendroff scheme updates each point with a weighted value of three points, two weights are positive, one negative. Hence, solution can contain oscillations with internal maxima and minima. Now consider smoother initial conditions:
![[Pasted image 20251031185839.png|centre|400]]
![[Pasted image 20251031185824.png|centre|400]]
