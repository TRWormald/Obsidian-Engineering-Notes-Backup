By considering a 'discrete' solution, stored (and updated) at only discrete points in space and time, we have derived two possible methods to update the solution.
We have obtained the finite-difference analogue of the original PDE:
$$\frac{\partial u}{\partial t}+c\frac{\partial u}{\partial x}=0$$
Which can be approximated by:
$$\frac{u_{i}^{n+1}-u_{i}^{n}}{\Delta t}+\frac{c}{\Delta x}(u_{i+1}^{n}-u_{i-1}^{n})+O(\Delta t, (\Delta x)^{2})=0$$
This uses a "central" difference in space. Alternatively we can use a one sided difference, i.e.
$$\frac{u_{i}^{n+1}-u_{i}^{n}}{\Delta t}+\frac{c}{\Delta x}(u_{i+1}^{n}-u_{i}^{n})+O(\Delta t, \Delta x)=0$$
or,
$$\frac{u_{i}^{n+1}-u_{i}^{n}}{\Delta t}+\frac{c}{\Delta x}(u_{i}^{n}-u_{i-1}^{n})+O(\Delta t, \Delta x)=0$$

### The Examination of Numerical Schemes
The scheme derived above (FTCS - Forward Time-Centred Space) is one of many possible ways we can discretise the equation numerically. We have derived the FTCS scheme by a rational mathematical approach, but how do we know that it will actually solve our equation?
It is obviously inefficient to examine every possible finite-difference stencil by coding it and then testing it. We need some measures:
1) The **order of accuracy** of the method is defined as the lowest power of $\Delta x$ and $\Delta t$ in the truncation error.
	Hence the FTCS scheme is 1st order accurate in time, and 2nd order accurate in space.
2) The **consistency** of the finite-difference analogue (FDA): a scheme is a formally consistent discretisation of the original PDE if the truncation error $\rightarrow 0$ as $\Delta x,~\Delta t\rightarrow 0$, in any way
3) The **stability** of a numerical scheme describes whether errors are amplified or reduced by the discrete scheme; a stable scheme damps out errors whilst an unstable scheme amplifies them
