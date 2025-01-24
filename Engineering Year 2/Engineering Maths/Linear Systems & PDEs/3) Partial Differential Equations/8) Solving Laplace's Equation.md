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
