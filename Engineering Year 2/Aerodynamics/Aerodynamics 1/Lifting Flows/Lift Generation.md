To evaluate lift it is easiest to work it out from first principles, we are effectively evaluating the forces on an element of surface formed by and angle $\delta\theta$ at $\theta$ from $x$:
![[Pasted image 20240429115004.png|center|250]]
So the pressure $p(\theta)$ is exerted over an area $R\delta\theta=\delta s$, however the force exerted contains both lift and drag components:
![[Pasted image 20240429115228.png|center|300]]
So resolving gives us that the lift is equal to:
$$\delta L =-p(\theta)\cdot R \delta\theta\cdot\sin\theta$$
Hence integrating this around the circle gives:
$$\begin{align*}
L&= -\int_{0}^{2\pi}p(\theta)R\sin\theta\cdot d\theta\\
&= -\int_{0}^{2\pi}(p(\theta)-p_{\infty}+p_{\infty})R\sin\theta\cdot d\theta\\\\
&= -\int_{0}^{\infty}(p(\theta)-p_{\infty})R\sin\theta\cdot d\theta-\int_{0}^{2\pi}p_{\infty}R\sin\theta\cdot d\theta
\end{align*}$$
The second integral evaluates to zero, allowing us to rewrite the equation as:
$$L=-\int_{0}^{\infty}(p(\theta)-p_{\infty})R\sin\theta\cdot d\theta$$
We know that the [[Engineering Year 1/AVDASI/Aerodynamics/Potential Flow/The Coefficient of Pressure - From Bernoulli's Equation|the Coefficient of Pressure]] is equal to:
$$C_{p}=\frac{p-p_{\infty}}{\frac{1}{2}\rho U_{\infty}^{2}}$$
So:
$$\frac{1}{2}\rho U_{\infty}^{2}C_{p}=p-p_{\infty}$$
Hence:
$$L=-\frac{1}{2}\rho U_{\infty}^{2}\int_{0}^{2\pi}C_{p}\sin\theta\cdot d\theta$$
We've already calculated our $C_{p}$ [[Engineering Year 2/Aerodynamics/Aerodynamics 1/Lifting Flows/Lifting Cylinder Flow#Calculating the Velocities and the Pressure Coefficient|here]] so:
$$L=-\frac{1}{2}\rho U_{\infty}^{2}\int_{0}^{2\pi}\left(1-4\sin^{2}\theta- \frac{2\Gamma\sin\theta}{U_{\infty}\pi R}-{\left(\frac{\Gamma}{2U_{\infty}\pi R}\right)^{2}}\right)\sin\theta\cdot d\theta$$
Which evaluates to:
$$L=\rho U_\infty\Gamma$$
Which is the general result for a 2D body with total 'bound' circulation $\Gamma$.