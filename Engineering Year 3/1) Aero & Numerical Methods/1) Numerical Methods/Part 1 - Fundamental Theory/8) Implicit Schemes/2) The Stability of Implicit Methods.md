Using the Von-Neumann Fourier stability analysis with the implicit scheme:
$$u_{i}^{n+1}=n_{i}^{n}-\nu_{i}(u_{i}^{n+1}-u_{i-1}^{n+1})$$
where as before:
$$\nu_{i}=\frac{c\Delta t}{\Delta x}$$
Substituting our Fourier representation gives:
$$u_{i}^{n+1}=u_{i}^{n}-\nu_{i}\left[e^{jki\Delta x}e^{-jkc(n+1)\Delta t}-\mathbf{e^{jk(i-1)\Delta x}}e^{-jkc(n+1)\Delta t}\right]$$
Expanding the bold term and then factorising our $e^{jki\Delta x}e^{-jkc(n+1)\Delta t}$ gives:
$$u_{i}^{n+1}=u_{i}^{n}-\nu_{i}u_{i}^{n+1}\left[1-e^{-jk\Delta x}\right]$$
Substituting $u_{i}^{n+1}=\lambda u_{i}^{n}$:
$$\lambda u_{i}^{n}=u_{i}^{n}-\nu_{i}\lambda u_{i}^{n}\left[1-e^{-jk\Delta x}\right]$$
We can then divide through by $u_{i}^{n}$ to give:
$$\lambda=1-\nu_{i}\lambda\left[1-e^{-jk\Delta x}\right]$$
From which we can substitute in the trigonometric identity:
$$\lambda =1-\nu_{i}\lambda(1-\cos(k\Delta x)+j\sin(k\Delta x))$$
and rearrange:
$$\frac{1}{\lambda}=1+\nu_{i}-\nu_{i}\cos(k\Delta x)+j\sin(k\Delta x)$$
And finally we can calculate the magnitude:
$$\left|\frac{1}{\lambda}\right|=\sqrt{1+2(\nu+\nu^{2})(1-\cos(k\Delta x))}$$
Hence the $|1/\lambda|$ can only be $\ge 1$ and so:
$$\lambda\le 1$$
for all values of $k, \nu$, i.e. the implicit method is unconditionally stable.
But why is this? Consider the difference between the stencils for explicit and implicit version of the first order upwind scheme:
![[Pasted image 20251102183409.png|centre|400]]
In the explicit scheme each point only receives information from two points over one time step, so the numerical domain of dependence is $\Delta x$. For implicit we have a matrix equation:
$$\mathbf{M \underline{u}}^{n+1}=\mathbf{\underline{u}}^{n}$$
And we can multiply by $\mathbf{M^{-1}}$ and multiply out row by row:
![[Pasted image 20251102183633.png|centre|500]]
etc.

The stability limit for explicit schemes comes from the stencil propagation. Each point only recieves information from the points in the F.D. stencil, and this gives a limit on the time step