Consider progressing the solution of:
$$\frac{\partial u}{\partial t}+c\frac{\partial u}{\partial x}=0$$
From time level $n$ to $n+1$ for $c>0$. The stable upwind scheme (backward difference) uses the stencil:
![[Pasted image 20251030191149.png|centre|400]]
i.e. only $u_{i}^{n}$ and $u_{i-1}^{n}$ can influence $u_{i}^{n+1}$ over one time step. However, over time $\Delta t$ the solution will propagate a distance $c\Delta t$. So the physical domain of dependence is $c\Delta t$. The numerical domain of dependence is limited to $\Delta x$ as the only information within one computational cell influences each point.
Consider three time step sizes, and the resulting influence:
![[Pasted image 20251030191416.png|centre]]
Hence, for the scheme to be stable, i.e. the correct information to influence each point, the numerical domain of dependence must be at least as large as the physical one:
$$\Delta x\ge c\Delta t$$
Or more commonly:
$$\frac{c\Delta t}{\Delta x}\le 1$$
This places a limit on the numerical time step. Clearly, the smaller we make the mesh spacing the more accurate our scheme becomes. But this then means that the time-step becomes smaller and we need more time-steps to reach a converged solution. Hence, increasing the number of mesh points increases the accuracy of the scheme, but costs twice - more time-steps on more points.