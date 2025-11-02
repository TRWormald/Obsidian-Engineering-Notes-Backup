Consider solving the linear wave equation,
$$\frac{\partial u}{\partial t}+c\frac{\partial u}{\partial x}=0$$
From a positive wavespeed, we can use the first order-upwind scheme,
$$\frac{u_{i}^{n+1}-u_{i}^{n}}{\Delta t}+\frac{c}{\Delta x}(u_{i}^{n}-u_{i-1}^{n})+O(\Delta t, \Delta x)=0$$
Which gives the resulting explicit updating scheme,
$$u_{i}^{n+1}=u_{i}^{n}-\frac{c\Delta t}{\Delta x}(u_{i}^{n}-u_{i-1}^{n})$$
Stability has shown that this is stable for:
$$\frac{c\Delta t}{\Delta x}\le 1$$
![[Pasted image 20251031124852.png|centre]]
![[Pasted image 20251031124938.png|centre]]![[Pasted image 20251031125022.png|centre]]
![[Pasted image 20251031125041.png|centre]]
The resulting solutions are shown below:
![[Pasted image 20251031125111.png|centre]]
Hence, the CFL = 0.75 solution shows dissipation, as λ < 1, the CFL = 1.0 solution models the solution exactly, as λ = 1 always, and the CFL = 1.5 solution is unstable. Over a 1.5 second timestep the solution should propagate 1.5 cells, but it is not possible for the numerical solution to propagate more than one cell over each timestep.
