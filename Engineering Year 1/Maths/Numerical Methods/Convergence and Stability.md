### Local and Global Error
**Local Error** - This is a measure of how wrong our approximation is when we take one timestep. If we knew $x_{n}$ exactly correctly, we define the local error as:
$$\text{local error} = |x_{n+1}-x(t_{n}+h)|$$
\
**Global Error** - This is a measure of the worst our approximation can be within a certain range of $t$ values. If we give initial conditions at $t_{0}=0$, we define the global error on the domain $0\le t \le T$ as:
$$\text{global error} = \max_{0\le n \le \frac{T}{h}}(|x_{n}-x(hn)|) $$
### Convergence
Consider the case where we want to approximate the solution to a first-order initial value problem:
$$\frac{dx}{dt}=f(x,t),~~~x(0)=x_{0}$$
If $x(t)$ is the true solution and $x_{n}$ is the approximation of the *n*th timestep, we say that a numerical method is **convergent** for $0<t<T$ if:
$$\text{global error}=\max_{0\le n\le \frac{T}{h}}(|x_{n}-x(hn)|)\rightarrow 0 \text{ as } h\rightarrow 0$$
In other words if the global error decreases as we decrease the step size, the method is convergent.
**Note: if $f(x,t)$ is a continuous function, the forward Euler meth**