Consider the explicit version of the FTCS scheme:
$$u_{i}^{n+1}=u_{i}^{n}-\frac{\nu}{2}(u_{i+1}^{n}-u_{i-1}^{n})$$
Which is unconditionally unstable. As with the upwind scheme, we switch from a forward to a backward temporal derivative (so the approximation is the same as the explicit), and the spatial derivative is approximated implicitly, to give:
$$u_{i}^{n+1}=u_{i}^{n}-\frac{\nu}{2}(u_{i+1}^{n+1}-u_{i-1}^{n+1})$$
Of course this is now backward time centred space at time level $n+1$. is this stable? Using the same stability analysis methods as before (find the full derivation on [[Numerical Methods Lecture 8.pdf#page=14|Numerical Methods Lecture 8, p.14]]) we obtain:
$$\left|\frac{1}{\lambda}\right|=\sqrt{1+\nu^{2}\sin^{2}(k\Delta x)}$$
and so:
$$\lambda\le1 $$
So for all values of $k$ and $\nu$ the implicit form of FTCS is unconditionally stable.