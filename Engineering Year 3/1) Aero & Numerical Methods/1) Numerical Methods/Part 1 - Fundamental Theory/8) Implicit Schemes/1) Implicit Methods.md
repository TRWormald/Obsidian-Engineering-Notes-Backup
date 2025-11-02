All the schemes we have considered so far have been explicit, i.e. only known values at the current time-level are required to update the solution at each point. 
Implicit schemes are fundamentally different, as they use "unknown" values of the solution at the next time-level to compute the solution at the next time-level.
Consider the linear wave equation again. We apprioximated the derivatives for the explicit scheme at the current time level as:
$$\left.\frac{\partial u}{\partial t}\right|_{i}^{n}+c\left.\frac{\partial u}{\partial x}\right|_{i}^{n}=0$$For implicit schemes the derivatives are approximated at the next time-level, i.e.
$$\left.\frac{\partial u}{\partial t}\right|_{i}^{n+1}+c\left.\frac{\partial u}{\partial x}\right|_{i}^{n+1}=0$$
Consider the first-order upwind scheme ($c>0$). The explicit scheme gives:
$$\frac{u_{i}^{n+1}-u_{i}^{n}}{\Delta t}+c\frac{u_{i}^{n}-u_{i-1}^{n}}{\Delta x}=0$$
For implicit schemes we approximate derivatives at the next time level. But since a backward difference at the next time level ($n+1$) is the same as a forward difference a the current time level, we end up with the same temporal difference formula.
Expand about $i$, $n+1$:
$$u_{i}^{n}=u_{i}^{n+1}-\Delta t\left.\frac{\partial u}{\partial t}\right|_{i}^{n+1}+ \frac{1}{2}(\Delta t)^{2}\left.\frac{\partial^{2} u}{\partial t^{2}}\right|_{i}^{n+1}+O(\Delta t^{3})$$
And so, neglecting terms of $O(t^2)$ we get:
$$u_{i}^{n}=u_{i}^{n+1}-\Delta t\left.\frac{\partial u}{\partial t}\right|_{i}^{n+1}+ O(\Delta t^{2})$$
or:
$$\left.\frac{\partial u}{\partial t}\right|_{i}^{n+1}=\frac{u_{i}^{n+1}-u_{i}^{n}}{\Delta t}$$
And so the implicit scheme is:
$$\frac{u_{i}^{n+1}-u_{i}^{n}}{\Delta t}+c\frac{u_{i}^{n+1}-u_{i-1}^{n+1}}{\Delta x}=0$$
This leads to a more complex equation to solve. The solution at each point cannot simply be updated using known values. At each time-step we get a set of equations which must be solved simultaneously. Consider the time-stepping ae each point.
Again we use:
$$\nu_{i}=\frac{c\Delta t_{i}}{\Delta x_{i}}$$
and so the scheme is:
$$u_{i}^{n+1}=n_{i}^{n}-\nu_{i}(u_{i}^{n+1}-u_{i-1}^{n+1})$$
To solve for each point we get a matrix equation,
![[Pasted image 20251102181134.png|centre]]
This is a very simple matrix, bidiagonal. Most schemes lead to a much more complex matrix equation to solve, tri- or penta-diagonal or sometimes sparse. 
Exact matrix inversion is very expensive, and it is normally done using approximate inversion techniques. 
Normally have to consider operator splitting or approximate factorisation, and these will be considered later in the course. Remember, for 3-D equations the matrix is (NI.NJ.NK)x(NI.NJ.NK). 
For realistic mesh dimensions it would not be possible to construct the matrix on a single machine, as there would not be sufficient memory. Normally need multi-node parallelism just for the memory requirement. 

>So if they are so complex, why do we use implicit schemes?
