Consider the initial problem:
$$\frac{dx}{dt}=x-x^{3}+cos(t),~~~~x(0)=1$$
We have no method for finding a closed-form solution to this ODE but we still want to understand its behaviour. Can we estimate the values of $x(t)$?
**Basic Method**:
- We know that $x(0)=1$, and we know that $x'(0)=1-1^{3}+cos(0)=1$
- We can use this information to get approximations for $x(t)$ when $t$ is close to zero.
- Based on these values of $x$, we can calculate vales of $x'$ at these points
- Based on these, we can calculate new approximations of $x$ at new $t$ values
- Keep repeating the process to expand the domain of the solution
#### Key Terminology
\
**Stepsize** - This is the difference between the $t$ values of adjacent points where we calculate approximations for $x$. We use $x_{n}\approx x(t_{0}+nh)$ to represent the approximation of $x$ at $n$ **timesteps** away from the initial condition. The stepsize is often written as $h$ or $\Delta t$.
\
**Method**- In the context of solving ODEs, a numerical method is a systematic way of going from the estimate of $x$ at one timestep to an estimate of $x$ at the next timestep.
Given a differential equation:
$$\frac{dx}{dt}=f(x,t)$$
and given $x_{n}$ as an approximation of $x(t_{0}+nh)$, a method is an algorithm that uses this information to obtain $x_{n+1}$, an approximation of $x(t_{0}+(n+1)h)$


