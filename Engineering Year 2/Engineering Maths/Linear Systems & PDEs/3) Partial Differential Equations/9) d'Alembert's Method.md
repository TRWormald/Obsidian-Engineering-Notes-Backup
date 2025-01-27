We have previously used [[5) Solving the Wave Equation#Summary of the Method of Separation|the separation of variables]] to find solutions to the wave equation:
$$\frac{\partial^{2}u}{\partial t^{2}}=c^{2}\frac{\partial^{2}u}{\partial x^{2}}$$
It is well suited to the case where we have **boundary conditions**. Then the spatial wavelength is determined by the boundary conditions. For example, what is the note played by the guitar string, the organ pipe, or a percussive instrument?
$$u(x,t)=\sum\limits_{n=1}^{\infty}b_{n}\sin\left(\frac{n\pi x }{L}\right)\cos\left(\frac{n\pi ct}{L}\right)$$
The solution is said to be a **standing wave**.
However this is not a viable method if the domain over which we solve the PDE is infinite.
What this means practically is that the domain is so large such that the boundaries are far away and cannot influence the wavelength.
Examples of this include ripples on a pond, or acoustic waves travelling through the ocean.
The kind of solution we are looking for is a **travelling wave**.
### The Travelling Wave Solution of the Wave Equation
In order to find travelling wave solutions we must note the following:

> **Theorem (d'Alembert's solution of the Wave Equation)**
> The function $u(x,t)$ given by:
> $$u(x,t)=f(x-ct)+g(x+ct)$$
> is a solution of the wave equation for any functions $f$ and $g$. It is made up of to travelling waves, with:
> 1) Fixed shape $f$, moving to the right, at speed $c$
> 2) Fixed shape $g$, moving to the left, at speed $c$

#### Proof of the Travelling Wave Solution
To begin the proof we just substitute the d'Alembert solution into the wave equation, to do this we need to find partial derivatives of $u(x,t)$ with respect of $x$ and $t$:
If $u(x,t)=f(x-ct)+g(x+ct)$ then:
$$\frac{\partial u}{\partial t}=\frac{\partial}{\partial t}f(x-ct)+\frac{\partial}
{\partial t} g(x+ct)$$
Make a change of variables so that: $\xi=x-ct$ $\eta=x+ct$, and use the chain rule:
$$\begin{align*}
&= \frac{\partial}{\partial t}f(\xi)+\frac{\partial}{\partial t}g(\eta)\\
&= \frac{\partial\xi}{\partial t}
\frac{d}{d\xi}f(\xi)+\frac{\partial\eta}{\partial t} \frac{d}{d\eta}g(\eta)\\
&= -cf'(\xi)+cg'(\eta)\\
&= -cf'(x-ct)+cg'(x+ct)\end{align*}$$
We can use the same technique to find all the partial derivatives of $u(x,t)=f(x-ct)+g(x+ct)$ with respect to $x$ and $t$:
$$u_t=-cf'(x-ct)+cg'(x+ct)$$
$$$$