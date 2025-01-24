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
#### Step 4 - Separating the Boundary/Initial Conditions
We can also separate the boundary and initial conditions, but only if they are **homogeneous** (i.e. function value equal to zero)
For example:
*If we have that $u$=0 at $x=0$ for all $t>0$, then:*
$$0=u(0,t)=X(0)T(t)$$
i.e. $u$ is a function of $x$ and $t$, with $x$ always being equal to zero, and therefore $u$ is always equal to zero. $t$ can be any value as it doesn't change the value of $x$ and hence the value of $u$.

Therefore either $X(0)=0$ or $T(t)=0$. The latter implies that:
$$u(x,t)=X(x)T(t)=0$$
Which can't be true. So we must have $X(0)=0$
If we separate the boundary ($u=0 \text{ at } x=0,L$ for all $t>0$) and initial conditions ($u_{t}=0$ at $t=0$ for all $0\le x\le L$) in the same way, we get:
$$X(0)=X(L)=0$$
$$T'(0)=0$$
#### Step 5 - Solve the Separated ODEs and apply Homogeneous Boundary Conditions
For a wave equation we need a $\mu<0$ so we write $\mu$ as $-k^2$ for some $k>0$. Then:
$$\left\{\begin{matrix}T''(t)=-(kc)^{2}T(t) \\ X''(x)=-k^2 X(x)\end{matrix}\right.~~~\Rightarrow~~~\left\{\begin{matrix}T(t)=A\cos(kct)+B\sin(kct) \\ X(x)=C\cos(kx)+D\sin(kx)\end{matrix}\right.$$
We then apply the separated boundary conditions for $X$. First at $x=0$:
$$X(0)=C\cos(k\cdot0)+D\sin(k\cdot0)$$
When $x=0$, $X(0)=C=0$, so applying that to when $x=x$:
$$X(x)=D\sin(kx)$$
And when $x=L$:
$$0=X(L)=D\sin(kL) \Rightarrow \sin(kL)=0$$
Therefore:
$$\boxed{kL=n\pi}$$ for some integer $n$.
Hence we can then solve for $k$:
$$k=\frac{n\pi}{L}$$
And also for the solution to the ODE:
$$X(x)=D\sin\left(\frac{n\pi x}{L}\right)$$
We also have that $T'(0)=0$ So recalling that:
$$T(t)=A\cos(kct)+B\sin(kct)$$
We can get that:
$$T'(t)=-kcA\sin(kct)=kcB\cos(kct)$$
Thus:
$$T'(0)=0=-kcA\cdot0+kcB\cdot 1=kcB$$
Which gives us $B=0$. Hence:
$$T(t)=A\cos(kct)$$
for some arbitrary constant A.
We also know that $k=n\pi/L$, so:
$$T(t)=A\cos\left(\frac{n\pi ct}{L}\right)$$
#### Step 6 - Putting the Pieces Together
From the solving of the ODEs we can combine them back to get the PDE:
$$u(x,t)=X(x)T(t)=b\sin\left(\frac{n\pi x}{L}\right)\cos\left(\frac{n\pi ct}{L}\right)$$
Where $b=AD$ is any constant, and $n$ is any integer. It satisfies the PDE and the homogeneous boundary and initial conditions, i.e:
$$u_{tt}=c^{2}u_{xx}$$
$$u(0,t)=0,~~~u(L,t)=0,~~~ u_{t}(x,0)=0$$
But not the non-homogeneous initial condition:
$$u(x,0)=f(x)$$
##### Linearity and the General Solution
The solution to the PDE that we've just found is valid for any integer $n$.
We can add any linear combination of them, with any integer values of $n$, and any multiplicative constant $b$, and still have a soltion.

So the general solution of the PDE + homogeneous boundary and initial conditions is:
$$u(x,t)=\sum\limits_{n=1}^{\infty}b_{n}\sin\left(\frac{n\pi x}{L}\right)\cos\left(\frac{n\pi ct}{L}\right)$$
This solution has infinitely many constants of integration $b_{n}$.
#### Step 7 - Applying the Non-Homogeneous Initial Conditions
We need to apply the initial condition:
$$u(x,0)=f(x),~~~~\text{for}~~~~0\le x\le L$$
Which gives:
$$u(x,0)\sum\limits_{n=1}^{\infty}b_{n}\sin\left(\frac{n\pi x}{L}\right)=f(x)$$
From this we want to find the $b_{n}$'s, given $f(x)$. *In fact we have already learnt how to do this, using a [[4) Odd and Even Periodic Extensions#The Half-Range Sine Series|Half Range Sine Series]]*
$$b_{n}=\frac{2}{L}\int_{0}^{L}f(x)\sin\left(\frac{n\pi x}{L}\right)~dx$$
So the particular solution to the PDE 