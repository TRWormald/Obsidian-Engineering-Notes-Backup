A second-order semi-linear PDE for $u(x,y)$:
$$A(x,y)\frac{\partial^{2}u}{\partial x^{2}}+B(x,y)\frac{\partial^{2}u}{\partial x ~\partial y}+C(x,y)\frac{\partial^{2}u}{\partial y^{2}}=f(x,y,u,u_x,u_y)$$
Can be classified into three different types:
- Parabolic equations for which $B^{2}-4AC=0$
- Hyperbolic equations for which $B^{2}-4AC>0$
- Elliptic equations for which $B^{2}-4AC<0$
The importance of this classification comes in the nature of the solutions that the different classes of PDE give rise to, and what kinds of boundary conditions are required.
### Parabolic PDEs
These are PDEs like the [[1) Introduction to PDEs#The Heat Equation|heat equation]]:
- They all have solutions that diffuse in a "time-like" independent variable
- They all have infinite speed information flow
- The solutions are generally smooth
To solve them we need:
- A single initial condition at a given time (e.g. a known initial temperature distribution)
- A pair of boundary conditions in the other (space-like) variable, one on each boundary (e.g. a known temperature at each end)
- Can be solved in an unbounded domain in the space like variable
### Hyperbolic PDEs
These are PDEs like the [[1) Introduction to PDEs#The Wave Equation|the wave equation]]:
- All have solutions that travel without decay along characteristic directions
- Information flows with well-defined finite speed
- Solutions can develop discontinuities (shock wave or steep fronts)
To solve them we need:
- Two initial conditions at a given time (e.g. a known temperature at each end)
- A pair of boundary conditions in the space-like variable, one on each boundary (e.g. known displacement at each end)
- Can be solved in an unbounded domain in the space-like variable
### Elliptic PDEs
These are PDEs like [[1) Introduction to PDEs#]]