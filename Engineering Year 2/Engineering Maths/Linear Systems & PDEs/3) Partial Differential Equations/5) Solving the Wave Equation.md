When solving a PDE using separation of variables we're going to assume that the solution is separable, i.e.
$$u(x,t)=X(x)T(t)$$
Substituting this assumption into the PDE will give us two separate ODEs: one for $X(x)$ and one for $T(t)$
The *homogeneous* boundary conditions will play a crucial role in  the solution process.

### Solving The Wave Equation
Consider the wave equation on a finite domain:
$$\underbrace{u_{tt}=c^{2}u_{xx}}_{\text{wave equation}}~~~~~~~~\underbrace{0\le x\le L,~~~t\ge0}_\text{finite domain}$$
subject to homogenous boundary conditions and initial conditions of known displacement and zero velocity:
$$\underbrace{u(0,t)=u(L,t)=0 \text{~for all } t>0}_{\text{boundary conditions}}$$
$$\underbrace{x(x,0)=f(x),~~u_{t}=(x,0)=0~\text{for all }0\le x\le L}_{\text{initial conditions}}$$
For some given (non-zero) function $f(x)$.

*Note that this means that the solution $u(x,t)\ne 0$, since its non-zero at time $t=0$* 
#### Stage 1 - Assume a Separable Solution
First, assume a separable solution:
$$u(x,t)=X(x)T(t)$$
Substituting this into the PDE we get:
$$\frac{\partial^{2}}{\partial t}[X(x)T(t)]=c^{2} \frac{\partial^{2}}{\partial x^{2}}[X(x)T(t)]$$
Which simplifies to:
$$X(x)T''(t)=c^{2}X''(x)T(t)$$
We can then divide both sides to get each side in terms of a single function and its derivatives:
$$\frac{1}{c^{2}}\frac{T''(t)}{T(t)}=\frac{X''(x)}{X(x)}$$
#### Stage 2 - The Separation Constant
The LHS of the equation above is a function of time only, while the RHS is a function of space only. But $x$ and $t$ are independent variables. This  can only be true if both are equal to a constant.
So:
$$\frac{1}{c^{2}}\frac{T''(t)}{T(t)}=\frac{X''(x)}{X(x)}=\text{constant}=\mu $$
Now we can separate the equations, into two separate ODEs, one for $X(x)$ and one for $T(t)$:
$$\left\{\begin{matrix}\frac{1}{c^{2}}\frac{T''(t)}{T(t)}=\mu \\  \frac{X''(x)}{X(x)}=\mu\end{matrix}\right.~~~~\Rightarrow\left\{\begin{matrix}T''(t)=\mu c^{2}T(t) \\ X''(x)=\mu X(x)\end{matrix}\right.$$
Where $\mu$ is the **separation constant**
#### Stage 3 - Solving the Separated ODEs
We can solve the separated ODEs for $X(x)$ and $T(t)$ if we know the sign of the separation constant $\mu$. There are two choices:
###### If $\mu>0$: 
Then we write $\mu=k^{2}$ for some $k>0$, then:
$$\left\{\begin{matrix}T''(t)=(kc)^{2}T(t) \\ X''(x)=k^2 X(x)\end{matrix}\right.~~~\Rightarrow~~~\left\{\begin{matrix}T(t)=Ae^{kct}+Be^{-kct} \\ X(x)=Ce^{kx}+De^{-kx}\end{matrix}\right.$$
###### If $\mu<0$: 
Then we write $\mu=-k^{2}$ for some $k>0$, then:
$$\left\{\begin{matrix}T''(t)=-(kc)^{2}T(t) \\ X''(x)=-k^2 X(x)\end{matrix}\right.~~~\Rightarrow~~~\left\{\begin{matrix}T(t)=A\cos(kct)+B\sin(kct) \\ X(x)=C\cos(kx)+D\sin(kx)\end{matrix}\right.$$
##### What Sign Should the Separation Constant Be?
Effectively:
- For the **wave equation** and the **heat equation** the separation constant must be negative
- For **Laplace's equation** it depends on the boundary conditions (more details later)
