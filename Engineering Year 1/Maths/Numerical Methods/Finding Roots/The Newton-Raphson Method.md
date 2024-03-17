The Newton-Raphson Method is another way of finding roots of equations numerically, it works similarly to the [[Fixed Point Iteration]] method but uses differentials instead:
![[Pasted image 20240316120851.png|center|400]]
*Let $f(x)$ be a differentiable function with a root $\alpha$ and let $x_{0}$ be an initial guess of $\alpha$. The Newton-Raphson Method is an iterative method for finding a root of $f$ given by:*
$$x_{n+1}=x_{n}-\frac{f(x_{n})}{f'(x_{n})}$$
It does not always does converge, but when it does it converges faster than most other frequently used iterative methods.
If $R_{n}=x_n-\alpha$, where $R_n$ is the error of the *n*th approximation. Newton's method typically gives $R_{n+1}\propto R_{n}^{2}$ (quadratic convergence).
