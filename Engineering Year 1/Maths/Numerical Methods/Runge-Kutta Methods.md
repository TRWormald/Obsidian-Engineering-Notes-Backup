### The Explicit Midpoint Method
One of the main types of Runge-Kutta methods is the 'explicit midpoint method'; it works similarly to the Euler method, but instead of finding the slope and then using it to calculate the next point we use it to find the point halfway between the current point and the next one in our iteration and then find the slope at that point before applying that to our original point:
![[Pasted image 20240321141948.png|center|500]]
Note how the slope at $x_\frac{1}{2}$ is parallel to the slope between $x_{0}$ and $x_{1}$.
#### Definition
The explicit midpoint method generates a numerical solution of an initial value problem using the iteration scheme:
$$x_{n+\frac{1}{2}}=x_{n}+ \frac{h}{2}f(x_{n},t_{n}),~~~x_{n+1}=x_n+hf\left(x_{n+ \frac{1}{2}},t_{n}+ \frac{h}{2}\right)$$
Where $x_{n+ \frac{1}{2}}$ is an intermediate value. Only $x_{n+1}$ is taken as part of our final estimate.
#### Error
The explicit midpoint method has local error $O(h^{3})$ and global error $O(h^{2})$. This is better than the Euler method as we know from [[The Euler Method#The Error of the Euler Method|the error of the Euler Method]]
#### Example
Use the explicit midpoint method, with stepsize $h=0.5$ to find $x(1)$ where $x$ is the solution of the initial value problem:
$$\frac{dx}{dt}=x,~~~x(0)=1$$
***
We know that $x_{0}=1$ and $t_{0}=0$ from the IVP.
\
First we take a half step:
$$x_\frac{1}{2}=x_{0}+ \frac{h}{2}f(x_{0},t_{0})=1+0.25\times1=1.25$$
Which we then use to find the full step:
$$x_{1}=x_{0}+hf(x_{\frac{1}{2}},t_{\frac{1}{2}})=1+0.5\times1.25=1.625$$
\
Repeating this process, now with $x(0.5)=x_{1}=1.625$ and $t_{1}=0.5$, the half step gives us:
$$x_{1+ \frac{1}{2}}=1.625+0.5\times 1.625=2.03125$$
Whilst using it to get the full step garners:
$$x(1)=x_{2}=1.625+0.5\times 2.03125=2.640625$$

