This is how we convert a higher order differential equation into a first order one to allow us to solve it using the Euler method:
A good example to demonstrate how to do this is a simple system with a constantly accelerating body.
We know that the acceleration can be described as:
$$\frac{d^{2}x}{dt^{2}}=a$$
However this cannot be numerically solved by the Euler method as it is not a first order differential equation.
We can get around this by creating a new variable:
$$v=\frac{dx}{dt}$$
Therefore:
$$\frac{dv}{dt}=\frac{d^{2}x}{dt^{2}}=a$$
Hence we get a system of first order differential equations:
$$\frac{dx}{dt}=v$$
$$\frac{dv}{dt}=a$$
We then use our standard method for [[The Euler Method For Systems of Differential Equations|solving systems of differential equations numerically using the Euler method]].
\
**Any ODE can be broken down in this way (into its first order components), and thus any ODE can be solved numercially.**
