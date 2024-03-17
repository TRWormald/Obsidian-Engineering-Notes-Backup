This is the equivalent of  [[The Degenerate Case (Or repeated roots)]] for a nonhomogeneous ODE.
##### Example
Take the ODE:
$$x'-x=e^t$$
We know that:
$$x=x_c+x_p$$
So:
$$x_c'-x_c=0$$
$$\lambda - 1 =0 \Rightarrow \lambda = 1$$
So:
$$x_c=Ce^t$$
As the function is exponential we make a guess that:
$$x_p=\alpha e^t$$And substitute it in:
$$\alpha e^t - \alpha e^t=e^t$$
But this give $e^t = 0$ which can never be true.
\
So we make another guess:
$$x_p=\alpha t e^t$$
Giving us:
$$\alpha e^t+\alpha t e^t-\alpha t e^t=e^t \Rightarrow \alpha e^t=e^t$$
Hence $\alpha=1$ and $x=Ce^t+te^t$

#####
The Problem: If the RHS of a non-homogeneous ODE satisfies the homogeneous equation then the normal guess for $x_p$ will not work
The Solution: Multiply the guess for $x_p$ by $t$ enough times to make it linearly independent.