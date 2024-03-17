A linear ODE of order $n$ with dependent variable $x$ and independent variable $t$ has constant coefficients if it can be written as:
$$a_n(t)\frac{d^nx}{dt^n}+a_{n-1}(t)\frac{d^{n-1}x}{dt^{n-1}}+\cdot\cdot\cdot+a_1(t)\frac{dx}{dt}+a_0(t)x=f(t)$$
Where the coefficients $a_n,a_{n-1},...$ do not depend on t (i.e. they are constant)
\
A linear homogeneous ODE with constant coefficients:
$$a_n(t)\frac{d^nx}{dt^n}+a_{n-1}\frac{d^{n-1}x}{dt^{n-1}}+\cdot\cdot\cdot+a_1(t)\frac{dx}{dt}+a_0(t)x=0$$
has at least one solution in the form $x=e^{\lambda t}$ where $\lambda$ is a constant.
If we substitute $x=e^{\lambda t}$ we get the **characteristic polynomial**:
$$a_n\lambda^n+a_{n-1}\lambda^{n-1}+\cdot\cdot\cdot+a_1\lambda+a_0=0$$
Where each root $\lambda_1,~\lambda_2,...$ of the characteristic polynomial gives a possible solution $x=e^{\lambda_i t}$.