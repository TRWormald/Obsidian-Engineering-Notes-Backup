When solving a PDE using separation of variables we're going to assume that the solution is separable, i.e.
$$u(x,t)=X(x)T(t)$$
Substituting this assumption into the PDE will give us two separate ODEs: one for $X(x)$ and one for $T(t)$
The *homogeneous* boundary conditions will play a crucial role in  the solution process.

### Solving The Wave Equation
Consider the wave equation on a finite domain:
$$\underbrace{u_{tt}=c^{2}u_{xx}}_{\text{wave equation}}~~~~~~~~\underbrace{0\le x\le L,~~~t\ge0}_\text{finite domain}$$
subject to homogenous boundary conditions and initial conditions of known displacement and zero velocity:
$$\underbrace{u(0,t)=u(L,t)=0 \text{~for all } t>0}_{\text{boundary conditions}}$$
$$\underbrace{x(x,0)=f(x),~~}_{\text{initial conditions}}$$
