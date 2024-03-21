The Euler method generates a numerical solution to an initial value problem given as:
$$\frac{dx}{dt}=f(x,t),~~~ x(t_{0})=x_{0}$$
in steps using the iteration scheme:
$$x_{n+1}=x_{n}+hf(x_{n},t_{n}),~~~t_{n+1}=t_{n}+h$$
Where $h$ is the stepsize.
### Example
Question: Find a numerical estimate of $x(1)$ where $x$ is the solution of the initial value problem:
$$\frac{dx}{dt}=x,~~~x(0)=1$$
using a stepsize of $h=0.25$.
\
So:
$$t_{0}=0,~~~x_{0}=1$$
$$t_{1}=t_{0}+h=0.25,~~~x_{1}=x_{0}+h\cdot f(x_{0},t_{0})=1+0.25\times 1=1.25$$
$$t_{2}=t_{1}+h=0.5,~~~x_{2}=x_{1}+h\cdot f(x_{1},t_{1})=1.25+0.25\times 1.25=1.56$$

$$t_{3}=0.75,~~~x_{3}=1.95$$

$$t_{4}=1,~~~x_{4}=2.44$$
Since $x(1)=2.718$ the error is $x(1)-x_{4}\approx -0.28$
### The Error of the Euler Method
The true solution of the initial value problem is $x(t)$ and a Taylor expansion around $t_{0}$ gives $x(t_{1})$ as a series:
$$x(t_{1})=x(t_{0})+x'(t_{0})(t_{1}-t_{0})+\frac{x''(t_{0})}{2}(t_{2}-t_{1})^{2}+...$$
In terms of $f$, $x_{0}$, and $h$ that is:
$$x(t_{1})=x_{0}+f(x_{0},t_{0})h+\frac{x''(t_{0})}{2}h^{2}$$
Which looks like the Euler scheme but with extra terms. The local error for $x_{1}$ is $x_{1}-x(t_{1})$ and:
$$x_{1}-x(t_{1})\approx\frac{x''(t_{0})}{2}h^2$$
So the error will decrease if we make the size of the steps smaller.
In other words the Euler Method has local error $O(h^{2})$ and global error $O(h)$.
### The Derivation
Given an initial value problem, with stepsize $h$:
$$\frac{dy}{dt}=f(t,y),~~~y(0)=y_{0}$$
We can approximate the gradient of this function by iterating $y$ by $h$ and finding the delta, and then dividing by $h$:
$$\frac{y(t+h)-y(t)}{h}\approx \frac{dy}{dt}=f(t,y)$$
If we consider what is going on here the function of $y$ is changing and we are calculating the change in it over an iteration of $h$ (so we are finding $\Delta y$), and $h$ is the change in the value along the x-axis ($t$), so we have $\frac{\Delta y}{\Delta x} =\text{grad}$.   
Rearranging to make $y(t+h)$ the solution of the equation:
$$y(t+h)=y(t)+hf(t,y(t))$$
Or in another form:
$$y_{n+1}=y_{n}+hf(t_{n},y_{n})$$
Which is our Euler method definition.