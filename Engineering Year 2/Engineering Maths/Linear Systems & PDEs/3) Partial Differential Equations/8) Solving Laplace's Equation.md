#### Laplace's Equation
Let's remind ourselves of [[1) Introduction to PDEs#Laplace's Equation|Laplace's Equation]]:
$$u_{xx}+u_{yy}=0$$
Since it only involves spatial coordinates, it is natural to pose Laplace's equation on domains of any shape. E.g. circular, or complex curvy shapres.
However, we shall concentrate on only the simplest case of a rectangular domain in 2D:
$$0<x<L,~~~0<y<M$$
##### Boundary Conditions for Laplace's Equation
We need one condition on each boundary ($x=0, L$ and $y=0,M$). There are two types we can pose:
- **Dirichlet**: $u$ is given on a boundary; e.g.
	- Homogeneous $u(0,y)=0$ for all $0\le y\le M$
	- Non-Homogeneous $u(x,0)=F(x)$ for all $0\le x \le L$
- **Neumann**: the normal derivative of $u$ is given on a boundary; e.g.
	- Homogeneous $u_{y}(x,M)=0$ for all $0\le x\le L$
	- Non-Homogeneous $u_{x}(L,y)=G(y)$ for all $0\le y\le M$
We'll focus on problems with three homogeneous boundary conditions and one non-homogeneous condition.
#### The Separation Constant for Laplace's Equation
To solve Laplace's equation, we look for a separable solution as usual:
$$u(x,y)=X(x)Y(y)$$
Substituting this into the PDE gives us:
$$X''(x)Y(y)+X(x)Y''(y)=0$$
Which simplifies to:
$$\frac{{X''(x)}}{X(x)}=-\frac{Y''(y)}{Y(y)}=\mu$$
**But what sign should $\mu$ take?**
Choosing the separation constant isn't quite as easy as for the heat and wave equations. The right choice depends on the homogeneous boundary conditions:

As usual there are two possibilities, either $\mu$ is negative or it is positive which gives different solutions to the ODEs:
If $\mu=-k^{2}<0$ then:
$$\left\{\begin{matrix}X''(x)=-k^{2}X(x) \\ Y''(y)=k^2 Y(y)\end{matrix}\right.~~~\Rightarrow~~~\left\{\begin{matrix}X(x)=A\cos(kx)+B\sin(kx) \\ Y(y)=Ce^{ky}+De^{-ky}\end{matrix}\right.$$
Or if $\mu=k^{2}>0$, so that: 
$$\left\{\begin{matrix}X''(x)=k^{2}X(x) \\ Y''(y)=-k^2 Y(y)\end{matrix}\right.~~~\Rightarrow~~~\left\{\begin{matrix}X(x)=Ce^{ky}+De^{-ky} \\Y(y)=A\cos(ky)+B\sin(ky)  \end{matrix}\right.$$

Since there is exactly one non-homogeneous boundary condition, that means that two opposite sides of the domain have homogeneous boundary conditions: $u$, or its normal derivative, equal to zero:
![[Pasted image 20250124180821.png|centre]]
In the first case above, separating the boundary conditions gives $X=0$ or $X'=0$ at both $x=0$ and $x=L$. So $X(x)$ must be $\sin$ and $\cos$ (i.e. when $\mu$ is less than zero).

In the second case separating the boundary conditions gives $Y=0$ or $Y'=0$ at both $y=0$ and $y=L$. So $Y(y)$ must be $\sin$ and $\cos$ (i.e. when $\mu$ is more than zero).
### Worked Example 5.2
