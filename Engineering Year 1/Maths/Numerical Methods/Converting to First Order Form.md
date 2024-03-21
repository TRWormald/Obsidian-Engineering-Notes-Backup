This is how we convert a higher order differential equation into a first order one to allow us to solve it using the Euler method:
A good example to demonstrate how to do this is a simple system with an accelerating body.
We know that the acceleration can be described as:
$$\frac{d^{2}x}{dt^{2}}=a$$
However this cannot be numerically solved by the Euler method as it is not a first order differential equation.
We can get around this by creating a 