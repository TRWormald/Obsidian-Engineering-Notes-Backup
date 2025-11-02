### Couette Flow Between a Fixed and Moving Plate
#### Assumptions
The assumptions we make are:
- 2D, incompressible, plane, viscous, axial flow
- Zero pressure gradient and gravity effects
- Fully developed flow (sufficiently far from the entrance)
![[Pasted image 20251029212956.png|centre|500]]
From the continuity equation:
$$\frac{\partial \rho}{\partial t}+\frac{\partial}{\partial x}(\rho u)+\frac{\partial}{\partial y}(\rho v)+\frac{\partial}{\partial z}(\rho w)=0$$
we obtain: $u=u(y)$, but how do we solve for this.
If we take our momentum equations we can effectively eliminate all of the terms, leaving us with:
$$\frac{\partial^{2}u}{\partial y^{2}}=0,~~~~~~~~u=C_{1}y+C_{2}$$
But then how do we solve for $C_{1}$ and $C_{2}$ - boundary conditions. At $y=+h$, we know that $U=V$, and at $y=-h$, we know that $U=0$.
Solving the above with these boundary conditions, we arrive at the solution for the Couette flow due to a moving wall:
$$u=\frac{V}{2h}y+ \frac{V}{2},~~~~\text{valid for }-h\le y\le +h$$
