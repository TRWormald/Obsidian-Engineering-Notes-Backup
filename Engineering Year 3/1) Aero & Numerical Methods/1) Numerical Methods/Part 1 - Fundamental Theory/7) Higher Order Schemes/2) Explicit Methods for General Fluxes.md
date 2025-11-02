So far we have only considered schemes for linear equations, i.e. constant wave speeds. The non-linear Burgers equation results in an FDA scheme for the first order upwind scheme:
$$\frac{\partial u}{\partial t}+\frac{\partial \left(\frac{1}{2}u^{2}\right)}{\partial x}=0$$
$$u_{i}^{n+1}=u_{i}^{n}-\frac{\frac{1}{2}(u_{i}^{n}+u_{i-1}^{n})\Delta t(u_{i}^{n}-u_{i-1}^{n})}{\Delta x}$$
where the "effective wavespeed" term is clear. Non-linear equations are normally written:
$$\frac{\partial u}{\partial t}+\frac{\partial F(u)}{\partial x}=0$$
which result in a first order upwind scheme of the form:
$$u_{i}^{n+1}=u_{i}^{n}-\frac{\Delta t}{\Delta x}(F(u_{i}^{n})-F(u_{i-1}^{n}))$$
which is written as:
$$u_{i}^{n+1}=u_{i}^{n}-\frac{\Delta t}{\Delta x}(F_{i}^{n}-F_{i-1}^{n})$$
However the Lax-Wendroff scheme for non-linear equations becomes more complex.
$$\frac{\partial u}{\partial t}+\frac{\partial F(u)}{\partial x}=0$$
We know as before:
$$u_{i}^{n+1}=u_{i}^{n}+\Delta t \left.\frac{\partial u}{\partial t}\right|_{i}^{n} +\frac{1}{2}(\Delta t)^{2}\left.\frac{\partial^{2}u}{\partial t^{2}}\right|_{i}^{n}+O(\Delta t^3)$$
and so again:
$$\left.\frac{\partial u}{\partial x}\right|_{i}^{n}=-\left.\frac{\partial F(u)}{\partial x}\right|_{i}^{n}=\frac{F_{i+1}^{n}-F_{i-1}^{n}}{2\Delta x}+O(\Delta x^{2})$$
But the second order term causes the problem:
![[Pasted image 20251031193453.png|centre|500]]
The spatial derivative do not cause any problems, but the $\frac{\partial F(u)}{\partial u}$ is complex to compute, and also it is not clear exactly where it should be evaluated. This then also has to be differentiated. This term is known as the Jacobian. For a system of $N$ equations, it is an $N\times N$ matrix.
### Example Jacobian: 1D Euler
We are normally concerned with systems of equations, for example the Euler or Navier-Stokes equations. For a system of N equations, the Jacobian is an N x N matrix. 1-D Euler equations are:
![[Pasted image 20251031193737.png|centre|300]]
Where,
$$E=\frac{P}{\gamma -1}+ \frac{1}{2}\rho u^{2}$$
These three equations are written as:
$$\frac{\partial \mathbf{U}}{\partial t}+\frac{\partial \mathbf{F}(\mathbf{U})}{\partial x}=0$$
Where $\mathbf{U}$ is the vector of conserved variables, and $\mathbf{F}$ is the flux vector:
![[Pasted image 20251031194001.png|centre]]
In this case the Jacobian would be (note that this is not examinable):
![[Pasted image 20251031194031.png]]
![[Pasted image 20251031194040.png|centre]]
### MacCormack's Method
A simpler higher order scheme is MacCormack's method. this is also a second order accurate scheme in time and space. to solve:
$$\frac{\partial u}{\partial t}+\frac{\partial F(u)}{\partial x}=0$$
MacCormack's scheme is a two stage scheme, known as a "predictor-corrector" method.
1) Predictor stage
$$u_{i}^\overline{n+1}=u_{i}^{n}-\frac{\Delta t}{\Delta x}(F_{i}^{n}-F_{i-1}^{n})$$
2) Corrector stage
$$u_{i}^{n+1}=\frac{1}{2}(u_{i}^{n}+u_{i}^\overline{n+1})-\frac{\Delta t}{2\Delta x}(F^{\overline{n+1}}_{i+1}=F^{\overline{n+1}}_{i})$$
In the above:
$$F^{\overline{n+1}}_{i+1}=F(u^{\overline{n+1}}_{i+1}),~~~etc.$$
By considering initially $F(u)=cu$ where $c$ is constant, i.e. the linear wave equation, we can show that MacCormack's Method is:
- Second order accurate in time and space
- Stable for CFL<1
- Consistent
Note that MacCormack's scheme is identical to the Lax-Wendroff method, but it is much simpler to code, as the Jacobian is not required.
### A Note on Wavespeeds
![[Pasted image 20251031195803.png]]![[Pasted image 20251031195834.png]]
![[Pasted image 20251031195900.png|centre]]
![[Pasted image 20251031195929.png]]
