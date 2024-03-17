The general solution of  the nonhomogeneous linear ODE:
$$a_n(t)\frac{d^nx}{dt^n}+a_{n-1}(t)\frac{d^{n-1}x}{dt^{n-1}}+\cdot\cdot\cdot+a_1(t)\frac{dx}{dt}+a_0(t)x=f(t)$$
takes the form $x(t)=x_c(t)+x_p(t)$, where $x_c(t)$ (the **complementary function**) is the general solution to the corresponding homogeneous ODE where $f(t)=0$, and $x_p(t)$ (the **particular integral**) is a particular solution to the nonhomogeneous ODE.
\
The particular solution is **any solution** for your differential equation, for example given the following differential equation:
$$\dot{x}+x=t$$
we know that the complementary function is going to be:
$$x_c=Ae^{-t}$$
so we need to find the particular integral, so:
$$\dot{x}_p+x_p=t$$
And what makes this true? If $x_p=t$ we would get $1+t=t$ which isn't true. So what about if we try $x_p=t-1$? Then we would get $1+t-1=t$ so that is our particular integral.
So the general solution to our differential equation would be:
$$x=Ae^{-t}+t-1$$
