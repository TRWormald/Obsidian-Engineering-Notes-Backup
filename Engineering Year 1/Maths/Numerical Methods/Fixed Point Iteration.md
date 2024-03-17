### The Basics
Let $g(x)$ be any real-valued function. We say that $c$ is a **fixed point** of $g$ if:
$$g(c)=c$$
Ife we are trying to find the root of a function $f(x)$, one possibility is to rearrange $f(x)=0$ into the form $g(x)=x$ and then apply $g$ iteratively on an initial guess, so that $x_{n+1}=g(x_n).$ In some cases this will lead to a  better and better approximation of the root of $f$. This process is called **fixed point iteration**.
For example given the following function to find the root of :
$$f(x)=x^4-3x+1$$
We would say that one of the possible fixed points is:
$$g(x)=\frac{x^4+1}{3}$$ As:
$$f(x)=0$$
Note that you can rearrange this to get a different fixed point, for some equations some fixed points will be convergent whilst others will be divergent.
### The Theory
*Fixed point iteration tries to estimate a solution $x'$ of the equation $x=g(x)$ using the iteration scheme $x_{n+1}=g(x_{n})$ and an initial guess $x_{0}$. For some function $g$ the sequence $x_{0},~x_{1},~x_{2},...$ moves away from the true solution $x'$ with each iteration no matter how close $x_{0}$ is to $x'$ (unless $x_{0}=x'$ exactly).*
\
**Guaranteeing Convergence**
*A fixed point iteration scheme $x_{n+1}=g(x_{n})$ will converge to a solution $x'$ if $x_0$ is sufficiently close to $x'$ and:*
$$0\ne\left|\frac{d}{dx}g(x')\right|<1$$
