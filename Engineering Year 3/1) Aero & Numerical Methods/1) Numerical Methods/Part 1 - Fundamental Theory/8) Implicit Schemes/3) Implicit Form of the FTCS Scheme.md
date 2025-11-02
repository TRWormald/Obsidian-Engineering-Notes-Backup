Consider the explicit version of the FTCS scheme:
$$u_{i}^{n+1}=u_{i}^{n}-\frac{\nu}{2}(u_{i+1}^{n}-u_{i-1}^{n})$$
Which is unconditionally unstable. As with the upwind scheme, we switch from a forward to a backward temporal derivative (so the approximation is the same as the explicit), and the spatial derivative ias approximated implicitly, to give